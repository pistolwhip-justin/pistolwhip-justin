# Obsidian Nest Vaults

Set up a folder in one vault to be its own vault in another location on your Windows file system. Obsidian treats each vault as an independent folder, so as long as you organize your vaults correctly, you can make this work.

Here’s how to set it up:

1. **Create or Identify the Folder**: In your existing vault, create a folder (e.g., `Project`) that you’d like to use as its own separate vault.

2. **Locate the Folder in File Explorer**: Find this folder on your file system. By default, Obsidian vaults are just folders with markdown files, so you can easily locate and open it in Windows Explorer.

3. **Create a New Vault in Obsidian**:
   - Open Obsidian, then go to **Open another vault** > **Open folder as vault**.
   - Select the `Project` folder from the file system.
   - Obsidian will now treat `Project` as an independent vault.

4. **Access and Manage Separately**: You can now open and manage `Project` as a standalone vault, independent from the original vault that contains it.

## Notes

- **File Changes**: Since both vaults access the same folder on the file system, any changes in one will reflect in the other.
- **Unique Configurations**: Settings, plugins, and appearance are independent for each vault, so you can customize each one as needed.
- **Vault Nesting**: Obsidian generally discourages nesting vaults within other vaults to avoid performance issues or potential conflicts. However, since you’re accessing `Project` as a separate vault, this setup should work smoothly as long as you’re mindful of overlapping files or configurations.

This setup can be useful for organizing content that you need to access in multiple contexts while keeping each vault’s configurations distinct.
