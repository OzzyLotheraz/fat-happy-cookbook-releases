# Fat & Happy Cookbook Releases

Public distribution repository for Fat & Happy Cookbook client releases and the published family cookbook data used by read-only clients.

## What belongs here

- Versioned Windows release artifacts and updater metadata.
- `cookbook/manifest.json`, which identifies the current published cookbook revision and hashes its payloads.
- `cookbook/recipes.json`, which contains the published read-only recipe collection.
- Published recipe media under `cookbook/media/` when recipes include local images.

## What must never be stored here

- Application source code.
- Admin credentials or publishing tokens.
- Development databases or private configuration.
- Unpublished/private recipes.

Windows and future Android clients may read the same published cookbook data. Application releases and cookbook revisions are intentionally independent, so recipe changes do not require a new application version.
