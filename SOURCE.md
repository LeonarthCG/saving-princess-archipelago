# Where is the source? Why should I trust this?

The source for gm-apclientpp.dll can be found over [at its repo](https://github.com/black-sliver/gm-apclientpp).

As for the source for the patch, unfortunately it cannot be provided, as doing so would mean including a bunch the game's original content.
However, I can walk you through getting something very close to what I use to work on the patch.

## Source at home

Here's a step-by-step:

- First of all, follow the instructions from the [setup guide](SETUP.md).
- Get [UndertaleModTool](https://github.com/UnderminersTeam/UndertaleModTool).
- Open the unpachted `original_data.win` with UndertaleModTool and run these scripts:
  * Scripts > Resource Unpackers > ExportAllCode.csx
  * Scripts > Resource Unpackers > ExportAllRoomsWithCC.csx
  * Scripts > Resource Unpackers > ExportAllSprites.csx
- Create a local repository with your favorite version control system and commit the files we extracted to it.
- Open the patched `data.win` with UndertaleModTool and run these scripts:
  * Scripts > Resource Unpackers > ExportAllCode.csx
  * Scripts > Resource Unpackers > ExportAllRoomsWithCC.csx
  * Scripts > Resource Unpackers > ExportAllSprites.csx
- Update your local repository with the new files.

And there you go, you now have something close to a recreation of the source. No comments, though.
