# Neovim Configuration Guidelines

## Commands
- Test: `<leader>t` (nearest), `<leader>T` (file), `<leader>a` (suite), `<leader>l` (last)
- Search: `<leader>sf` (files), `<leader>sg` (grep), `<leader>sh` (help)
- Format: `<leader>f` (format buffer)
- LSP: `gd` (definition), `gr` (references), `<leader>ca` (code action)

## Code Style
- Indentation: 2 spaces (controlled by vim-sleuth)
- Max line length: ~80-100 characters
- Naming: snake_case for variables, PascalCase for types/classes
- Error handling: Use pcall for protected calls to handle errors gracefully
- Imports: Group by standard library, external plugins, local modules

## Formatting
- Lua: stylua
- Python: isort, black
- JavaScript/TypeScript: prettier
- Ruby: standardrb

## Project Structure
- `/lua/custom/plugins/` - User plugins
- `/lua/kickstart/` - Base configuration modules