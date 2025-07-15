# MacOS Setup

- [Checklist](#checklist)
- [How to install (In Order)](#how-to-install-in-order)
- [To be config:](#to-be-config)
  - [Home \& End key](#home--end-key)
  - [Oh-my-zsh + Powerlevel10k](#oh-my-zsh--powerlevel10k)
  - [iTerm2](#iterm2)


## Checklist

### Fix mac
- Mac Mouse Fix
- Balance Lock
- iTerm2
- Oh-my-zsh  
- Powerlevel10k

### Package manager
- Homebrew
- PNPM

### Font
- Fira Code

### Dev
- Git
- Sourcetree
- VSCode
- Figma

## How to install (In Order)

<table>

<tr>
<td>Mac Mouse Fix</td>
<td><a href="https://github.com/noah-nuebling/mac-mouse-fix/tags">https://github.com/noah-nuebling/mac-mouse-fix/tags</a></td>
</tr>

<tr>
<td>Balance Lock</td>
<td><a href="https://www.tunabellysoftware.com/balance_lock/">https://www.tunabellysoftware.com/balance_lock/</a></td>
</tr>

<tr>
<td>Raycast</td>
<td><a href="https://www.raycast.com/">https://www.raycast.com/</a></td>
</tr>

<tr>
<td>Homebrew</td>
<td><a href="https://brew.sh/">https://brew.sh/</a></td>
</tr>

<tr>
<td>PNPM</td>
<td><a href="https://pnpm.io/installation">https://pnpm.io/installation</a></td>
</tr>

<tr>
<td>git</td>
<td><code>brew install git</code></td>
</tr>

<tr>
<td>Sourcetree</td>
<td><a href="https://www.sourcetreeapp.com/">https://www.sourcetreeapp.com/</a></td>
</tr>

<tr>
<td>VSCode</td>
<td><a href="https://code.visualstudio.com/Download">https://code.visualstudio.com/Download</a></td>
</tr>

<tr>
<td>Figma</td>
<td><a href="https://www.figma.com/downloads/">https://www.figma.com/downloads/</a></td>
</tr>

<tr>
<td>Fira Code</td>
<td><br>

```sh
brew install font-hack-nerd-font
brew install --cask font-fira-code font-fira-code-nerd-font
```

</td>
</tr>

<tr>
<td>iTerm2</td>
<td><a href="https://iterm2.com/downloads.html">https://iterm2.com/downloads.html</a></td>
</tr>

<tr>
<td>oh-my-zsh</td>
<td><a href="https://ohmyz.sh/">https://ohmyz.sh/</a></td>
</tr>

<tr>
<td>Powerlevel10k</td>
<td><a href="https://github.com/romkatv/powerlevel10k">https://github.com/romkatv/powerlevel10k</a></td>
</tr>

</table>

## To be config

### Home & End key

Create `~/Library/KeyBindings/DefaultKeyBinding.dict` with below content

```js
{
  "\UF729"  = moveToBeginningOfParagraph:; // home
  "\UF72B"  = moveToEndOfParagraph:; // end
  "$\UF729" = moveToBeginningOfParagraphAndModifySelection:; // shift-home
  "$\UF72B" = moveToEndOfParagraphAndModifySelection:; // shift-end
  "^\UF729" = moveToBeginningOfDocument:; // ctrl-home
  "^\UF72B" = moveToEndOfDocument:; // ctrl-end
  "^$\UF729" = moveToBeginningOfDocumentAndModifySelection:; // ctrl-shift-home
  "^$\UF72B" = moveToEndOfDocumentAndModifySelection:; // ctrl-shift-end
}
```

### Oh-my-zsh + Powerlevel10k
Copy `.zshrc`, `.p10k.zsh` to `$HOME`

### iTerm2
Import `Tokyo Night.json`
