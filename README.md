# Magento Patch Exporter

This is a small utility that's designed to export patched from a Magento distribution to a given folder.

## Usage

```bash
php magento-patcher /path/to/magento /path/to/export
```

It works by reading `app/etc/applied.patches.list` of a given Magento installation (`/path/to/magento`). It'll then collate all of the patched files and spit them out to the export path (`/path/to/export`), recreating their file structure.

## Limitations

This tool assumes that `/path/to/export` exists and that it's empty. Maybe one day I'll make provisions to create this path on the fly and remove the contents of it.
