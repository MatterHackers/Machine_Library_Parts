# Machine_Library_Parts
Digital library parts (stls and other data) for each of the machines that MatterControl knows about (profiles)

## Only Upload AMF files
All meshes added to this repository should be .amf files. They have both shared vertices and are compressed. They are often 1/20th the size of the same mesh saved as an STL.

## Layout
- Folders for each Make
  - Name must mach MatterControl's
- Folders for each Model
  - Within Make folders
  - Name must  mach MatterControl's

## File Types
- AMF files
- STL files
- Image files (PNG, JPG, etc.)
- .library files
  - You can upload library files to link to other GitHub repositories that can be viewed as folders in MatterControl

## Library File format
A .library file has the following content.
```
{
  "type": "GitHub",
  "owner": "MatterHackers",
  "repository": "PulseOpenSource",
  "path": "C Frame"
}
```
- "type" - Always set to "GitHub" (it can also be 'local' when used on a client machine)
- "owner" - The GitHub account that owns the repository to be read
- "repository" - The repository name that is part of the "owner"s repositories
- "path" - The local path to a specific folder within the "repository", can be left as "" to show the entire "repository"

The name preceding the .library extension will be the name displayed for the folder within MatterConrtrol
