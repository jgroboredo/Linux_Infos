# 1. Table of contents

- [1. Table of contents](#1-table-of-contents)
  - [1.1. Introduction](#11-introduction)
- [2. Markdown Notes](#2-markdown-notes)
  - [2.1. VsCode extensions](#21-vscode-extensions)
- [3. Git notes](#3-git-notes)
  - [3.1. Notes on creating a git repository on github](#31-notes-on-creating-a-git-repository-on-github)
    - [3.1.1. Some notes on the above commands](#311-some-notes-on-the-above-commands)
  - [3.2. Check previous commit](#32-check-previous-commit)
  - [3.3. Git stash and log](#33-git-stash-and-log)
  - [3.4. Create local git repository](#34-create-local-git-repository)
  - [3.5. Change the author name](#35-change-the-author-name)
  - [3.6. Remove tracked file that is now in .gitignore](#36-remove-tracked-file-that-is-now-in-gitignore)
  - [3.7. Check last commit changes](#37-check-last-commit-changes)
  - [3.8. Installing git in live ISO arch](#38-installing-git-in-live-iso-arch)
  - [3.9. Change remote URL](#39-change-remote-url)
  - [3.10. Add remote URL](#310-add-remote-url)
  - [3.11. Different Pushes](#311-different-pushes)
  - [3.12. Download a file from github](#312-download-a-file-from-github)
  - [3.13. Merge branches](#313-merge-branches)
  - [3.14. Check merge conflicts](#314-check-merge-conflicts)
  - [3.15. Merge mistake (You committed changes to (local) master)](#315-merge-mistake-you-committed-changes-to-local-master)
  - [3.16. Git merge "Deleted by us"](#316-git-merge-deleted-by-us)
  - [3.17. Commit ID and SHA](#317-commit-id-and-sha)
  - [3.18. Git over ssh using ssh config](#318-git-over-ssh-using-ssh-config)
  - [3.19. Sparse Checkout](#319-sparse-checkout)
  - [3.20. Git submodules](#320-git-submodules)
    - [3.20.1. Add submodule](#3201-add-submodule)
    - [3.20.2. Clone repo with submodule](#3202-clone-repo-with-submodule)
    - [3.20.3. Pulling in Upstream Changes from the Submodule Remote](#3203-pulling-in-upstream-changes-from-the-submodule-remote)
    - [3.20.4. Pulling Upstream Changes from the Project Remote](#3204-pulling-upstream-changes-from-the-project-remote)
    - [3.20.5. Upstream repository changed url of the submodule](#3205-upstream-repository-changed-url-of-the-submodule)
    - [3.20.6. Switching from subdirectories to submodules](#3206-switching-from-subdirectories-to-submodules)
  - [3.21. Migrate part of git repository](#321-migrate-part-of-git-repository)
- [4. Bash Notes](#4-bash-notes)
  - [4.1. Bash Note 1](#41-bash-note-1)
  - [4.2. Bash Note 2](#42-bash-note-2)
  - [4.3. Bash Note 3](#43-bash-note-3)
  - [4.4. Bash Note 4 - Compare Files](#44-bash-note-4---compare-files)
  - [4.5. Bash Note 5 - Use of curly braces](#45-bash-note-5---use-of-curly-braces)
  - [4.6. Bash Note 6 - Search recursively in directory](#46-bash-note-6---search-recursively-in-directory)
- [5. Lyx](#5-lyx)
  - [5.1. Configure lyx](#51-configure-lyx)
  - [5.2. Kpathsea](#52-kpathsea)
  - [5.3. Configure minted](#53-configure-minted)
  - [5.4. Install custom cls](#54-install-custom-cls)
- [6. Qemu](#6-qemu)
  - [6.1. Commands](#61-commands)
  - [6.2. Variables](#62-variables)
- [7. Inkscape](#7-inkscape)
- [8. VsCode](#8-vscode)
- [9. Zathura](#9-zathura)
- [10. Zsh](#10-zsh)
- [11. Jupyter](#11-jupyter)
  - [11.1. Jupyter-Lab](#111-jupyter-lab)
  - [11.2. Opening browser](#112-opening-browser)
- [12. Tmux](#12-tmux)
- [13. Pacman](#13-pacman)
  - [13.1. Pacman cache](#131-pacman-cache)
  - [13.2. Install from live usb](#132-install-from-live-usb)
  - [13.3. Pacman infos](#133-pacman-infos)
  - [13.4. pacman mirrors](#134-pacman-mirrors)
- [14. Grub](#14-grub)
  - [14.1. Install grub manually when manjaro fails](#141-install-grub-manually-when-manjaro-fails)
- [15. Vim](#15-vim)
  - [15.1. Install Vim in cluster](#151-install-vim-in-cluster)
  - [15.2. Vim snippets](#152-vim-snippets)
  - [15.3. Manage Tabs](#153-manage-tabs)
  - [15.4. Vim surroundings](#154-vim-surroundings)
  - [15.5. Some commands](#155-some-commands)
- [16. Lighdm](#16-lighdm)
- [17. i3Blocks](#17-i3blocks)
- [18. PcmanFM](#18-pcmanfm)
  - [18.1. Basic Configuration](#181-basic-configuration)
- [19. MPV](#19-mpv)
  - [19.1. Annoying bar at the top](#191-annoying-bar-at-the-top)
  - [19.2. Watch stream](#192-watch-stream)
- [20. Mime-Types](#20-mime-types)
  - [20.1. Alternative to xdg:](#201-alternative-to-xdg)
- [21. Color-Scheme](#21-color-scheme)
- [22. LibreOffice](#22-libreoffice)
- [23. Reflector](#23-reflector)
- [24. AceStream](#24-acestream)
- [25. Swig](#25-swig)
- [26. TTY Login](#26-tty-login)
  - [26.1. Add Username](#261-add-username)
  - [26.2. Change startup message](#262-change-startup-message)
- [27. HPC](#27-hpc)
  - [27.1. Modules](#271-modules)
  - [27.2. Some Commands](#272-some-commands)
- [28. Network](#28-network)
  - [28.1. Network not connecting at startup](#281-network-not-connecting-at-startup)
  - [28.2. MAC address](#282-mac-address)
- [29. Dmenu\_ext](#29-dmenu_ext)
  - [29.1. Not opening paths](#291-not-opening-paths)
- [30. Nvidia](#30-nvidia)
  - [30.1. NVIDIA back screen on TTY](#301-nvidia-back-screen-on-tty)
- [31. CFP Nvidia](#31-cfp-nvidia)
  - [31.1. VPN access](#311-vpn-access)
  - [31.2. First steps to config account](#312-first-steps-to-config-account)
- [32. Awk](#32-awk)
- [33. Sublime-Text](#33-sublime-text)
- [34. Config-Printer](#34-config-printer)
  - [34.1. CUPS](#341-cups)
  - [34.2. AVAHI](#342-avahi)
  - [34.3. HP SCANNER](#343-hp-scanner)
- [35. Sway](#35-sway)
  - [35.1. Packages to check for base arch install](#351-packages-to-check-for-base-arch-install)
  - [35.2. Services](#352-services)
  - [35.3. Sway install from YT:](#353-sway-install-from-yt)
  - [35.4. Sway my experience](#354-sway-my-experience)
    - [35.4.1. Packages](#3541-packages)
    - [35.4.2. Configuration](#3542-configuration)
    - [35.4.3. Fix cannot open display](#3543-fix-cannot-open-display)
    - [35.4.4. Mathematica](#3544-mathematica)
    - [35.4.5. Zoom](#3545-zoom)
    - [35.4.6. Albert](#3546-albert)
- [36. Rclone](#36-rclone)
  - [36.1. Config](#361-config)
  - [36.2. Rclone union](#362-rclone-union)
  - [36.3. Problem](#363-problem)
  - [36.4. Sync](#364-sync)
  - [36.5. OneDrive](#365-onedrive)
- [37. Pipewire](#37-pipewire)
- [38. Fail2Ban](#38-fail2ban)
  - [38.1. Configuration](#381-configuration)
- [39. Systemd-User](#39-systemd-user)
- [40. Systemd-Resolved](#40-systemd-resolved)
  - [40.1. Activate Service:](#401-activate-service)
  - [40.2. systemd-networkd](#402-systemd-networkd)
- [41. Dual Boot](#41-dual-boot)
  - [41.1. Windows After Linux](#411-windows-after-linux)
  - [41.2. Fix Windows bootloader Gone](#412-fix-windows-bootloader-gone)
- [42. RP Monitor](#42-rp-monitor)
  - [42.1. Create db in influxdb](#421-create-db-in-influxdb)
  - [42.2. CONFIG GRAFANA](#422-config-grafana)
  - [42.3. Notes](#423-notes)
- [43. Docker](#43-docker)
  - [43.1. Jacket](#431-jacket)
  - [43.2. Sonarr](#432-sonarr)
    - [43.2.1. Add manually downloaded season](#4321-add-manually-downloaded-season)
  - [43.3. System service to run docker](#433-system-service-to-run-docker)
  - [43.4. Rclone DLNA](#434-rclone-dlna)
  - [43.5. Transdrone](#435-transdrone)
  - [43.6. JellyFin](#436-jellyfin)
  - [43.7. QBitTorrent](#437-qbittorrent)
  - [43.8. Bazarr](#438-bazarr)
  - [43.9. Organizrr](#439-organizrr)
  - [43.10. NginX](#4310-nginx)
  - [43.11. Some Important Concepts](#4311-some-important-concepts)
  - [43.12. Update Containers](#4312-update-containers)
  - [43.13. Some notes based on experience](#4313-some-notes-based-on-experience)
- [44. VPN](#44-vpn)
  - [44.1. Configuration](#441-configuration)
  - [44.2. Notes](#442-notes)
  - [44.3. Viseu](#443-viseu)
  - [44.4. Check Ports](#444-check-ports)
  - [44.5. Fix connection problem](#445-fix-connection-problem)
  - [44.6. Connect to Rebelo](#446-connect-to-rebelo)
  - [44.7. Allow access to my VPN on another VPN](#447-allow-access-to-my-vpn-on-another-vpn)
  - [44.8. UDP2RAW](#448-udp2raw)
  - [44.9. Updated VPN](#449-updated-vpn)
  - [44.10. Fixing routes](#4410-fixing-routes)
  - [44.11. Rebelo's Jellyfin](#4411-rebelos-jellyfin)
- [45. DDNS](#45-ddns)
- [46. Encrypt dir](#46-encrypt-dir)
  - [46.1. Disable password cache](#461-disable-password-cache)
- [47. Violent Monkey](#47-violent-monkey)
- [48. Wireshark](#48-wireshark)
- [49. Telegram](#49-telegram)
  - [49.1. BotFather](#491-botfather)
  - [49.2. Find bot chat ID](#492-find-bot-chat-id)
  - [49.3. Add sonarr and radarr to telegram](#493-add-sonarr-and-radarr-to-telegram)
- [50. Barrier](#50-barrier)
- [51. TeamViewer](#51-teamviewer)
- [52. Flatpak](#52-flatpak)
  - [52.1. Firefox](#521-firefox)
- [53. VM](#53-vm)
  - [53.1. Fix Resolution](#531-fix-resolution)
  - [53.2. SDcard on VM](#532-sdcard-on-vm)
- [54. Latex](#54-latex)
- [55. Plex](#55-plex)
- [56. Format phone](#56-format-phone)
  - [56.1. Formatting](#561-formatting)
  - [56.2. Connecting to PC](#562-connecting-to-pc)
  - [56.3. ARCH LINUX IN TERMUX](#563-arch-linux-in-termux)
  - [56.4. Process to format](#564-process-to-format)
  - [56.5. Apps ADB](#565-apps-adb)
- [57. Find Command](#57-find-command)
  - [57.1. Error with mv command](#571-error-with-mv-command)
- [58. Conky Desktop](#58-conky-desktop)
  - [58.1. Install conky-manager](#581-install-conky-manager)
- [59. EndeavourOS Stuff](#59-endeavouros-stuff)
  - [59.1. Relativamente ao barrier](#591-relativamente-ao-barrier)
- [60. Map Keyboard Keys](#60-map-keyboard-keys)
- [61. Format Pen](#61-format-pen)
  - [61.1. Apagar partições](#611-apagar-partições)
  - [61.2. Criar Partição](#612-criar-partição)
  - [61.3. Format pen with ISO](#613-format-pen-with-iso)
- [62. Borg Backup](#62-borg-backup)
  - [62.1. Setup Steps](#621-setup-steps)
  - [62.2. MOUNT BACKUP AUTOMATICALLY](#622-mount-backup-automatically)
- [63. HDD Format](#63-hdd-format)
  - [63.1. Delete Partitions](#631-delete-partitions)
  - [63.2. Create New GPT partition table](#632-create-new-gpt-partition-table)
  - [63.3. Format Disk](#633-format-disk)
  - [63.4. Find UUID and check type](#634-find-uuid-and-check-type)
  - [63.5. Fstab](#635-fstab)
- [64. Ubuntu](#64-ubuntu)
  - [64.1. Fix ethernet unavailable](#641-fix-ethernet-unavailable)
- [65. PROBLEM: Unknown fs type vfat](#65-problem-unknown-fs-type-vfat)
  - [65.1. Some notes](#651-some-notes)
- [66. Permissions](#66-permissions)
  - [66.1. Fix permissions](#661-fix-permissions)
- [67. Raspberry Pi](#67-raspberry-pi)
- [68. Plasma](#68-plasma)
  - [68.1. Packages](#681-packages)
  - [68.2. Launch](#682-launch)
  - [68.3. Autostart](#683-autostart)
  - [68.4. XDG Autostart directories](#684-xdg-autostart-directories)
  - [68.5. Autostart Manager](#685-autostart-manager)
  - [68.6. Disable kdeconnect](#686-disable-kdeconnect)
  - [68.7. Shortcuts](#687-shortcuts)
  - [68.8. Fixing hanging service on shutdown](#688-fixing-hanging-service-on-shutdown)
  - [68.9. Config](#689-config)
    - [68.9.1. Startup and Shutdown → Background Services](#6891-startup-and-shutdown--background-services)
    - [68.9.2. Startup and Shutdown → Desktop Session](#6892-startup-and-shutdown--desktop-session)
    - [68.9.3. Power Management → Energy Saving](#6893-power-management--energy-saving)
    - [68.9.4. Display and Monitor → Night Color](#6894-display-and-monitor--night-color)
    - [68.9.5. Window Management → Task Switcher](#6895-window-management--task-switcher)
    - [68.9.6. FlameShot](#6896-flameshot)
    - [68.9.7. Task Bar](#6897-task-bar)
- [69. Regex](#69-regex)
- [70. Compare files](#70-compare-files)
- [71. Fiddler](#71-fiddler)
- [72. Termux](#72-termux)
  - [72.1. Termux Brightness](#721-termux-brightness)
  - [72.2. TV url opener](#722-tv-url-opener)
- [73. VPN Critical](#73-vpn-critical)
- [74. Secure Boot](#74-secure-boot)
  - [74.1. Steps for secure boot](#741-steps-for-secure-boot)
- [75. Helix](#75-helix)
  - [75.1. Some commands](#751-some-commands)
- [76. Pihole](#76-pihole)
  - [76.1. Configuration](#761-configuration)
- [77. Thunderbird](#77-thunderbird)
  - [77.1. Critical Account](#771-critical-account)
    - [77.1.1. Configure](#7711-configure)
    - [77.1.2. Calendar](#7712-calendar)
- [78. XDG-DESKTOP-PORTAL](#78-xdg-desktop-portal)
- [79. Parsec](#79-parsec)
  - [79.1. Wake on lan](#791-wake-on-lan)
  - [79.2. Wake PC](#792-wake-pc)
- [80. Misc](#80-misc)

## 1.1. Introduction

In this document I include some notes about general stuff I learn and do during my work/free time.

<div style="page-break-after: always; break-after: page;"></div>

# 2. Markdown Notes

## 2.1. VsCode extensions

- Markdown all in One
  - `Ctrl + Shift + P: Markdown All in One: section numbers, create table of contents, etc`
- Markdown lint
- vscode-pandoc
  - Ctrl + Shift + P -> Pandoc Render
  - Add `"pandoc.pdfOptString": "-t html --css style.css"` to `settings.json` in `.vscode/settings.json` in the work directory containing the markdown project. This `settings.json` overrides the global variables specified in that file. This can also be edited by doing `Ctlr+Shift+P: Preferences: Workspace Settings`. The `style.css` is put in the same folder of the `.md` file
  - `pacman -S pandoc pandoc-crossref wkhtmltopdf
- Markdown PDF  
  We can add to the `setting.json` for vscode workspace to use a specific style to generate the pdf:
```
  "markdown-pdf.styles": [
          "style.css",
      ],
```

<div style="page-break-after: always; break-after: page;"></div>

# 3. Git notes

## 3.1. Notes on creating a git repository on github  

On folder do:

```bash
 git init
 git commit
 git branch -M main
 git remote add origin https://github.com/jgroboredo/test.git
 git push -u origin main
```

### 3.1.1. Some notes on the above commands

- `git branch -m master main`

 > renames the master branch in local git repository

- In the second step, we'll have to create a new branch on the remote named "main" - because Git does not allow to simply "rename" a remote branch. Instead, we'll have to create a new "main" branch and then delete the old "master" branch:
`git push -u origin main`
We now have a new branch on the remote named "main".
- When you clone a repository with git clone , it automatically creates a remote connection called origin pointing back to the cloned repository.
- When you do a git push origin master, you are saying to git: "Look git, I want to push the current branch I am on to the remote repository named origin, and I want to push to the master branch in that remote.". By default, the remote repository is named origin. I only need to specify where I want to push if there are more than 1 repositories.
- When you execute the command: git remote add origin "github repo link" you are saying that for the current project, there is a remote repository with the name origin, with the address of "github repo link"

## 3.2. Check previous commit  

```
 git log
 git checkout <commit_hash> (example: 18e0b6a044a715b04bcacd599061b6b8bd586a7a)
 git checkout <branch_to_return_to_present_state>
```

## 3.3. Git stash and log  

```
 git log --stat -> see which files were altered in each commit
 git stash; git stash list; git stash drop
```

## 3.4. Create local git repository  

- Create a folder which is going to be the "server" -> For example, Notes.git
- Inside the repository do: `git init --bare`
- On the same computer do: `git clone /path/to/server`   -> the repository created this way will be linked to the "server" by an absolute path which only works on this same pc
- On the other computer do: `git clone goncalo@ip:/path/to/server`

## 3.5. Change the author name  

`git config --global user.name "John Doe"`

## 3.6. Remove tracked file that is now in .gitignore  

`git rm --cached <file>`

## 3.7. Check last commit changes  

 `git show --name-only` -> Lists just the files in the last commit and doesn't give you the entire guts
`git diff HEAD^ HEAD` -> HEAD^ identifies last commit

## 3.8. Installing git in live ISO arch  

 If error in keys: `pacman -Sy archlinux-keyring; pacman-key --populate archlinux`

## 3.9. Change remote URL  

- `git remote -v`

> To check the present remote url

- `git remote set-url origin git@github.com:jgroboredo/Linux_Infos.git`

## 3.10. Add remote URL  

- `git remote add name_of_remote git@github.com:jgroboredo/Linux_Infos.git`
- `git push -u name_of_remote --all`

> Note: this changes the default repository! It also pushes all branches!

- `git config --edit`

> Can use this command to change the default git push

- `git branch --set-upstream-to <remote-name>`

> Set preferred remote for current branch

- `git branch branch_name --set-upstream-to <remote-name>/branch`

> set preferred remote for branch_name

- `git branch -vv`

> shows the default remote for the current branch

## 3.11. Different Pushes  

- To push all branches to all remotes:
  `git remote | xargs -L1 git push --all`
- Push a specific branch to all remotes:
  `git remote | xargs -L1 -I R git push R branch_name`
- To make a git alias for the command:
  `git config --global alias.pushall '!git remote | xargs -L1 git push --all'`

Or

- Create an all remote with several repo URLs to its name:

```
 git remote add all origin-host:path/proj.git
 git remote set-url --add all nodester-host:path/proj.git
 git remote set-url --add all duostack-host:path/proj.git
 git push all --all
```

Or

- If you want to always push to repo1, repo2, and repo3 but always pull only from repo1, set up the remote 'origin' as:

```
 git remote add origin https://exampleuser@example.com/path/to/repo1
 git remote set-url --push --add origin https://exampleuser@example.com/path/to/repo1
 git remote set-url --push --add origin https://exampleuser@example.com/path/to/repo2
 git remote set-url --push --add origin https://exampleuser@example.com/path/to/repo3
```

- If you only want to pull from repo1 but push to repo1 and repo2 for a specific branch specialBranch:

```
  [remote "origin"]
     url = ssh://git@aaa.xxx.com:7999/yyy/repo1.git
     fetch = +refs/heads/*:refs/remotes/origin/*
     ...
  [remote "specialRemote"]
     url = ssh://git@aaa.xxx.com:7999/yyy/repo1.git
     pushurl = ssh://git@aaa.xxx.com:7999/yyy/repo1.git
     pushurl = ssh://git@aaa.xxx.com:7999/yyy/repo2.git
     fetch = +refs/heads/*:refs/remotes/origin/* (Note: Has origin here again, only pulls from origin)
     ...
  [branch "specialBranch"]
     remote = origin
     pushRemote = specialRemote
     ...
```

- My experience:
  - I can specify which remote to push or pull from:

      ```bash
      git pull remote_name branch
      git push remote_name branch
   ```

  - A branch has a default remote: I only need to specify the remote_name and eventually the branch_name (I can't pull from a non-default remote without specifying the branch) if I don't want to do it to the default one

## 3.12. Use curl to download from github  

```bash
curl -LkSs https://api.github.com/repos/jgroboredo/arch_install/tarball -o master.tar.gz
tar xf master.tar.gz
```

## 3.12. Download a file from github  

- Go to file, click on raw, copy link
- `curl -L "link_from_above_step" >> output`

## 3.13. Merge branches  

- `git checkout master; git merge other_branch_name`
- Alternative:`git merge --no-ff other_branch_name` . Using --no-ff allows someone reviewing history to clearly see the branch you checked out to work on.
- `git branch -d branch_name`  

> deletes branch locally

- `git push origin --delete branch_name`

> deletes a branch remotely

- `git fetch -p`

> Synchronize branch listing. After fetching, branches which no longer exist on the remote will be deleted.

If I do a: `git pull origin master` on another branch, it will merge them.
After creating a new branch, we need to specify tracking information for the current branch. That means we need to do something like `git pull <remote> <branch>` for it to work.
On the other hand, we can simply set tracking information for the current branch by:
`git branch --set-upstream-to=origin/<branch> correction_chapter1`

## 3.14. Check merge conflicts  

`git show --name-only [commit sha]` on a commit that was a merge containing conflicts and you'll see it as part of the message.

## 3.15. Merge mistake (You committed changes to (local) master)  

```
git branch <new-branch>
git reset HEAD~ --hard
git checkout new-branch 
```

The first command creates the new branch we want to work with. The second command resets the main branch to just before the last commit, but leaves the changes you just made in the new branch. Finally, we switch to the new branch where your changes await you.
If you’ve made multiple commits, use `git reset HEAD~<n> --hard`, where <n> is the number of commits back you want to go.

## 3.16. Git merge "Deleted by us"  

Resolve all non deleted merge conflicts by hand, which you have to do anyway;
Type `git diff --name-only --diff-filter=U` to get a list of all remaining files in conflit. These files must be the ones you want deleted.
`git diff --name-only --diff-filter=U | xargs git rm`

## 3.17. Commit ID and SHA  

```bash
git show -s --format=%H # shows the last commit full id
git show -s --format=%h # shows the last commit sha
```

## 3.18. Git over ssh using ssh config  

`git remote set-url origin ssh://pi(here config name)/home/goncalo/HDD/Documents/git_repos/Notes.git` (here full path)

## 3.19. Sparse Checkout

```bash
mkdir <repo>
cd <repo>
git init
git remote add -f origin <url>
```

This creates an empty repository with your remote, and fetches all objects but doesn't check them out.

Then: `git config core.sparseCheckout true`

Now we define which files/folders we want to check out by editing `.git/info/sparse-checkout`:

```bash
echo "some/dir/" >> .git/info/sparse-checkout
echo "another/sub/tree" >> .git/info/sparse-checkout
```

Finally, just update the repo: `git pull origin master`

## 3.20. Git submodules

### 3.20.1. Add submodule

```bash
# Add submodule to repository
# By default, submodules will add the subproject 
# into a directory named the same as the repository

git submodule add <link_to_submodule> <optional_path>

# Although the submodule is a subdirectory in your working directory,
# Git sees it as a submodule and doesn’t track its 
# contents when you’re not in that directory

git diff --cached --submodule
```

### 3.20.2. Clone repo with submodule

```bash
git clone <main_project_link>
git submodule init # initializes local config file
git submodule update # fetch all the data from that project

# or

git clone --recurse-submodules

# or
git clone <main_project_link>
git submodule update --init
```
### 3.20.3. Pulling in Upstream Changes from the Submodule Remote

```bash
cd <git_submodule_dir>
git fecth
git merge

# or

git submodule update --remote <submodule_name>

cd <main_project>
git diff --submodule #  get a list of commits that were added to the submodule
git config --global diff.submodule log # to avoid the need to write --submodule in every git diff

# If you commit at this point then you will lock the submodule 
# into having the new code when other people update.

git config -f .gitmodules submodule.DbConnector.branch stable # in order to track other branch

# if we leave off -f .gitmodules it will only make the change locally

git config status.submodulesummary 1 # to see a summary of changes to the submodules
```

### 3.20.4. Pulling Upstream Changes from the Project Remote

Now the perspective of the colaborator that cloned the Main Project.

Simply executing `git pull` is not enough. 
By default, the git pull command recursively fetches submodules changes. However, it does not update the submodules. 

```bash
git submodule update --init --recursive

# --init flag: MainProject might have added new submodules
# --recursive flag: if submodules have nested submodules

# or 

git pull --recurse-submodules
```

### 3.20.5. Upstream repository changed url of the submodule

```bash
# copy the new URL to your local config
$ git submodule sync --recursive
# update the submodule from the new URL
$ git submodule update --init --recursive
```

### 3.20.6. Switching from subdirectories to submodules

Problem:  we have been tracking files in our project and want to move them out into a submodule.

```bash
#First unstage
git rm -r SubDir
# Then Add
git submodule add <submodule_link>
```

## 3.21. Migrate part of git repository

After a fresh clone of the repository to migrate, do:

```bash
git-filter-repo --prune-degenerate always --prune-empty always --path /path/to/keep/1 --path /path/to/keep/2 

# Eventually rename things
# Put everything in root
git-filter-repo --path-rename /previous/path/:

# Change name
git-filter-repo --path-rename /previous/path/:/new/path

# migrate to new repo
cd new_repo
git init
git remote add old-repo ../myrepo
git pull old-repo master --allow-unrelated-histories
git remote remove old-repo
git add origin <new/origin>
```

<div style="page-break-after: always; break-after: page;"></div>

# 4. Bash Notes

## 4.1. Bash Note 1
- `$#`
  > number of arguments passed to the shell script
- `$1, $2`, etc
  > identify the arguments passed to the script

## 4.2. Bash Note 2
The code:

```bash
case $1 in
  -f|--from) command1; shift ;;
  *)         command2;;
  esac
  shift
```

will check if the first argument `$1` passed to the script matches `-f` or `--from` or any other cases; The asterisk means that it does command2 if it doesn't match any of the cases above;
The "shift" command shifts the arguments, i.e., if I have `$1`, `$2` arguments, then `$2` -> `$1`.

## 4.3. Bash Note 3
The code:

`SCRIPT_DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" &> /dev/null && pwd )"`

will give you the full directory name of the script no matter where it is being called from.

## 4.4. Bash Note 4 - Compare Files

`grep -F -x -v -f fileA fileB`
> This works by using each line in `fileA` as a pattern (`-f fileA`) and treating it as a plain string to match (`-F`). You force the match to happen on the whole line `-x` and print out only the lines that don't match (`-v`). Therefore, you are printing out the lines in fileB that don't contain the same data as any line in fileA.

## 4.5. Bash Note 5 - Use of curly braces

1) In the example:

```bash
  var=10        # Declare variable

  echo "${var}" # One use of the variable
  echo "$var"   # Another use of the variable
```

it makes no difference to use curly braces.

2) However, the `{}` in `${}` are useful if you want to expand the variable foo in the string `"${foo}bar"` since "$foobar" would instead expand the variable identified by foobar.

Curly braces are also unconditionally required when:

- expanding array elements, as in `${array[42]}`
- using parameter expansion operations, as in `${filename%.*}` (remove extension)
- expanding positional parameters beyond 9: `"$8 $9 ${10} ${11}"`

## 4.6. Bash Note 6 - Search recursively in directory

- `grep -R "stuff"` will search recursively on all files on that directory and look for the word stuff
- `for i in **/.ipynb_checkpoints` will find recursively all directories with this name
- `for i in ./pattern` will search for this pattern in current directory

<div style="page-break-after: always; break-after: page;"></div>

# 5. Lyx

## 5.1. Configure lyx

- Tools-Preferences-File Formats: PDF (pdflatex), shortname: pdf2, Viewer: Custom - zathura
- Tools-Preferences-Output-PDF command: `zathura --synctex-forward $$n:1:$$t $$o`
- Tools-Preferences-Shortcuts-New: buffer-view pdf2 and buffer-update pdf2
- For the spellchecker, might need to install hunspell-en_US and hunspel-pt_pt and enchant
- For lgrenc.def not found -> install texlive-langgreek
- To use eps figures in lyx I need ghostscript : try to epstopdf on command line to discover this.

## 5.2. Kpathsea

- Kpathsea is a library for path searching (e.g., for very quickly locating a given .sty file in a set of potentially large TEXMF trees, without doing a recursive directory tree trversal every time a given file is needed. (pse -> pathsea)
- kpsewhich minted.sy to search efficiently on tex library

## 5.3. Configure minted

```bash
sudo mkdir "/usr/share/texmf-texlive/tex/latex/minted/"
sudo cp minted.sty "/usr/share/texmf-texlive/tex/latex/minted/"
sudo mktexlsr
```

- Then in lyx, go to Tools/Tex Information, select latex styles and click rescan. minted.sty should appear in the list in lyx, go to "Tools>preferences>file handling>converters" and find the converter from tex to pdflatex. Edit its command line adding the option "-shell-escape" (no quotes) into the Converter field, then click the Modify button next to the list of converters. This is equivalent to going to Documents->Formats->Allow running external programs (is a better solution since it avoids writting a warning message). Then click Apply in lyx, go to Document>Settings and enter "/usepackage{minted}" (no quotes) in the latex preamble in lyx, in the part of your document where you want the highlighted code to appear, go to "Insert>TEX code" to get an Evil Red Text (ERT) box
- In Document->Settings->Listings, add following options:
  - language=C++
  - frame=single
  - mathescape=true
  - `syoek --synctex-forward $$n:1:$$t $$o`

- Ordered bibliography: Use style unsrt and add to preamble: \usepackage{notoccite}

## 5.4. Install custom cls

- `latex my_class.ins` -> produces my_class.cls
- `kpsewhich -var-value=TEXMFHOME` -> prints path where to put cls
- Regarding the above command, it's good to put the usual path: `$HOME/texmf/tex/latex/commonstuff/`
- kpsewhich my_class.cls -> to check path of the class
- Write lyx layout: In order to do this, find the basis class for our new class. For that, inspect my_class.cls and check the line LoadClass. It implies that my_class.cls is a descendent of that class (let's suppose it's dependent on report class). Then, in /usr/share/lyx/layouts copy report.layout, change its name to my_class.layout and edit like this:

```
  \DeclareLaTeXClass[my_class]{name_of_layout}
  Input report.layout
```

- In lyx, reconfigure. Now, name_of_layout is the text we see in Document-Class
- Default classes: `/usr/share/texmf-dist/latex/elsarticle/elsarticle.cls`

<div style="page-break-after: always; break-after: page;"></div>

# 6. Qemu

## 6.1. Commands

```bash
qemu-img create -f qcow2 qemu_image 8G
qemu-system-x86_64 -smp 6 -m 4G -enable-kvm -cdrom arch.iso -boot order=d qemu_image
smp (number of cores)

qemu-system-x86_64 -soundhw ac97 -k en-us -vga std -enable-kvm -m 4G  -usbdevice tablet -smp 6 -enable-kvm -boot c qemu_image
#For no sound
qemu-system-x86_64 -k en-us -vga std -enable-kvm -m 4G  -usbdevice tablet -smp 6 -boot c qemu_image
```

## 6.2. Variables

```bash
-k en-us (keymap)
-usbdevice tablet

-cpu host
-smp 6 # number of cores
-machine type=pc,accel=kvm
-enable-kvm
-format=raw ??
-machine smm=off # bug?
-soundhw sb16,es1370

#telnet access
qemu-system-x86_64 -curses -monitor telnet:127.0.0.1:1234,server,nowait -boot c qemu_image
telnet 127.0.0.1 1234  -- in another terminal

#KVM Quick Check
zgrep CONFIG_VIRTIO /proc/config.gz
lsmod | grep kvm
```

<div style="page-break-after: always; break-after: page;"></div>

# 7. Inkscape

- If I have problems with eps images, in this case, also need to install ghostscript.
- Do you have ImageMagick installed? LyX relies on ImageMagick to convert among graphics formats. It also needs Ghostscript installed (IM uses GS when the conversions involve PS, EPS or PDF files).
- If `textext` package form the AUR gives problem, simply go to **textext** official website and install it from there

<div style="page-break-after: always; break-after: page;"></div>

# 8. VsCode

- You can format an entire file with Format Document (Ctrl+Shift+I)  or just the current selection with Format Selection (Ctrl+K Ctrl+F) in right-click context menu.
- F1 -> command pallet
- SSH : F1 -> Remote-SSH: Connect to Host...
- Install extension: TabNine
  
<div style="page-break-after: always; break-after: page;"></div>

# 9. Zathura

- `pacman -S zahtura-pdf-poppler`
- make zathura default pdf viewer: `mimeo --ad application/pdf zathura.desktop`
- to discover the real name of zathura.desktop run `locate zathura.desktop`
- to check that pdf files have the correct mimetype run `mimeo -m pdf_file.pdf`
- Clipboard: add `set selection-clipboard clipboard` to `~/.config/zahtura/zathurarc` or `/etc/zathurarc`

<div style="page-break-after: always; break-after: page;"></div>

# 10. Zsh

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh in .zshrc
mkdir .cache/zsh && touch .cache/zsh/dirs
```

<div style="page-break-after: always; break-after: page;"></div>

# 11. Jupyter

## 11.1. Jupyter-Lab

To run over ssh, execute

```bash
ssh -L 8888(port on local):localhost::8889(port on remote) goncalo@ip jupyter-lab --no-browser --port=(same as before on remote)8889
```

- To avoid authentication by token: `jupyter server password`
- To list active sessions: `jupyter lab list`
- To kill a session: `jupyter lab stop 8888` (for e.g.)

## 11.2. Opening browser

If jupyter doesn't open, do :
`jupyter lab build`
If command above gives permission error, do:

```bash
sudo chown -hR {user} {dir}
jupyter notebook (lab) --generate-config 
```

Also, change redirect_file to false
Na verdade, isto não funciona porque tenho de mudar o `~/.profile` para firefox LOL

---

- Can't access file (probably happens cause directory contains hidden folder .local):
  - set `c.ServerApp.use_redirect_file = False` in `~/.jupyter jupyter_server_config.py`
  - Stop server:
  ```bash
      lsof -n -i4TCP:[port-number]
      kill -9 [PID]
  ```

<div style="page-break-after: always; break-after: page;"></div>

# 12. Tmux

ssh host, tmux, run command, `ctr+b d`, exit. To check the tmux session, run `tmux attach`

<div style="page-break-after: always; break-after: page;"></div>

# 13. Pacman

- Update pacman mirrors: `reflector --verbose --latest 5 --sort rate --save /etc/pacman.d/mirrorlist`
- Check recently installed packages: `grep -i installed /var/log/pacman.log`

## 13.1. Pacman cache

```bash
sudo ls /var/cache/pacman/pkg/ | wc -l # checks cached packages
du -sh /var/cache/pacman/pkg/ # disk space occupied by cache
sudo paccache -r # cleans all packages except most recent 3
sudo paccache -rk 1 # keep only one most recent version
sudo pacman -Sc # remove all uninstalled packages
sudo pacman -Scc # remove installed and uninstalled packages from cache
sudo paccache -ruk0 #**** remove all versions of uninstalled packages
change /etc/pacman.conf ParallelDownloads=5
```

## 13.2. Install from live usb

```bash
mount system: mount /dev/sdax /mnt
sudo pacman --root /mnt -S package
sudo pacman -Qkk | grep warning # To verify the presence of the files  installed by a package
sudo pacman --root /mnt -S $(sudo pacman --root /mnt -Qeq) --noconfirm # reinstalls installed packages
#If need to remove aur packages:
sudo pacman --root /mnt -Qeq > packages.txt
sudo pacman --root /mnt -S $(cat packages.txt) --noconfirm
```

## 13.3. Pacman infos

```bash
pacman -Qe # lists explicitly installed packages
pacman -Rsc # uninstalls (including unneeded dependencies)
pacman -Qs "query" # search installed packages for keywords
pacman -Qdt # list unneeded packages
pacman -Rns $(pacman -Qdtq) # uninstall unneeded packages (nota: quando adicionei isto aos aliases, sempre que abri o terminal pedia-me a pass do sudo (estava a correr o que esta a frente de $)
```

## 13.4. pacman mirrors
`sudo pacman-mirrors --fasttrack && pacman -Syyu`

<div style="page-break-after: always; break-after: page;"></div>

# 14. Grub

- If no update-grub command, do:
  ```bash
  sudo nano /usr/sbin/update-grub
  "
  #!/bin/sh
  set -e
  exec grub-mkconfig -o /boot/grub/grub.cfg "$@" 
  "
  sudo chown root:root /usr/sbin/update-grub
  sudo chmod 755 /usr/sbin/update-grub
  ```

- If error syntax in grub-customizer:
  - View -> Show placeholders
  - select entry "script code"
  - remove
- check kernel by `uname -r`


## 14.1. Install grub manually when manjaro fails
- Deactivate CSM in BIOS
- Quando acaba a instalacao, ver se ele cria a particao em /boot/efi ou /boot
- `sudo fdisk --list` (para ver onde foi instalada a particao no pc)
- `sudo su`
- `mount /dev/sda2 /mnt` (em que sda2 era a particao com o linux)
- `mount /dev/sda1 /mnt/boot/efi`
- `grub-install --target=x86_64-efi --efi-directory=/mnt/boot/efi --bootloader-id=manjaro --boot-directory=/mnt/boot --recheck --debug`
- `manjaro-chroot -a`
- `update-grub`
- `umount -R /mnt`

[Link](https://forum.manjaro.org/t/manjaro-grub-install-error-calamares-and-manual-the-why/125886)

<div style="page-break-after: always; break-after: page;"></div>

# 15. Vim

- `yay -S vim-plug-git`
- add `.vimrc` with the plugs I want
- add folder `~/.vim/plugged/`
- to install plugs, do `:PlugInstall`
- for fzt pluggin: `:Files` command
- For the NERDTree plugin to see icon of file, install: `yay -S nerd-fonts-complete`;
This font package my screw up font sizes of icons. To correct this, add to i3blocks config the following:

```
	<span size='small' font_weight='light'> icon </span> 
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;And change font on terminal to SauceCodePro Nerd Font Medium

- To open a file in a new tab in nerdtree, press t (or T); to open vertically click s;
- To cycle through windows: C-W-W, C-W-H, C-W-L, C-W-J, C-W-K
- To open file using fzf do:
- CTRL+T to open in new tab
- CTRL+X to open a new split
- CTRL+V to open in a new vertical split
- While in NERDTree, click on "m" to have a menu to do stuff with the file or other things
- `yay -S vim-youcompleteme-git` -> vim autocompletion (Needs to be done separately from the installation of the dotfiles)
- No need to add this plugin (vim-youcompleteme-git) to the `.vimrc` file
- add: `let g:ycm_show_diagnostics_ui = 0` to disable error checking by YouCompleteMe
- `pacman -S python-black`

## 15.1. Install Vim in cluster

```bash
git clone https://github.com/vim/vim.git
./configure --prefix=$HOME/.local && make && make install
# More flags: --disable-perlinterp --enable-rubyinterp --enable-multibyte --enable-pythoninterp --with-features=huge
export PATH="/home/youruser/.local/bin:$PATH"
# For plugins:
mkdir .vim/autoload
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Place in `.vimrc` before `plug#begin()`:

```
let data_dir = has('nvim') ? stdpath('data') . '/site' : '~/.vim'
if empty(glob(data_dir . '/autoload/plug.vim'))
    silent execute '!curl -fLo '.data_dir.'/autoload/plug.vim --create-dirs  https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
    autocmd VimEnter * PlugInstall --sync | source $MYVIMRC
endif
```

## 15.2. Vim snippets

- `:UltiSnipsEdit` command opens up a custom snippets file for the current language/filytype
- Don't need the above step if I install vim-snippets plugin

## 15.3. Manage Tabs
- To move tabs -> `Alt + arrows`
- To merge tabs -> `Ctr + m` or `Ctrl + n`;
- To exchange position of merged tabs -> `<C-w> x`;
- To change cursor position -> `<C-w> w`;
- To rotate windows -> `<C-w> <C-r>`

## 15.4. Vim surroundings

- cs(atual)(target) -> change surround from "atual" to "target"
- ds"  -> delete surround "
- ysiw[ -> yank surround inner word [ -> puts [ surrounding the word the curson is in
- ysf(smth)[ -> puts [ surrounding current cursor position till smth


## 15.5. Some commands

- procurar coisas: /searchthing e usa-se n ou N para avançar para as seguintes
- procurar string e substituir:
  
```
  :s/search/replace/
  :8,10 s/search/replace/g procura nas linhas 8 a 10
  :%s/search/replace/g procura no documento inteiro
  :%s/search/replace/gc pede confirmação para alterar
```

- copiar e colar:
selecionar o texto, y copia, p cola

<div style="page-break-after: always; break-after: page;"></div>

# 16. Lighdm

```text
pacman -S lightdm-gtk-greeter-settings
change default greeter: /etc/lightdm/lightdm.conf under [Seat:*]
pacman -S archlinux-wallpaper
pacman -S materia-gtk-theme
yay -S pop-icon-theme-git
yay -S pop-gtk-theme
```

<div style="page-break-after: always; break-after: page;"></div>

# 17. i3Blocks

For the scripts to work, even if it is .py, need to chmod +x
- https://github.com/vivien/i3blocks-contrib/tree/master/
- For calendar, install yad and xdotool; add:
`for_window [class='Yad'] floating enable`

<div style="page-break-after: always; break-after: page;"></div>

# 18. PcmanFM

## 18.1. Basic Configuration
- Go to edit -> Preferences -> Advanced :
  - Set terminal emulator (ex: xfce4-terminal) -> to open directly with vim for example
  - Set archiver integration: xarchiver

- To see thumbnails, install the following packages:
  - poppler-glib
  - ffmpegthumbnailer
  - freetype2
  - raw-thumbnailer
  - tumbler
  - libgsf
  - libgepub

<div style="page-break-after: always; break-after: page;"></div>

# 19. MPV

## 19.1. Annoying bar at the top

- Change picom config: frame-opacity option

## 19.2. Watch stream

- `pacman -S yt-dlp`
- `mpv 'link'`

<div style="page-break-after: always; break-after: page;"></div>

# 20. Mime-Types

## 20.1. Alternative to xdg:

- `yay -S mimeo`
- `yay -S xdg-utils-mimeo` 

[MIMEO COMMANDS](https://xyne.archlinux.ca/projects/mimeo/)

- Open files (foo, bar, etc) : `mimeo foo bar baz`
- find Leafpad's desktop file: `mimeo --app2desk leafpad`
- determine "test" file's MIME-type: `mimeo -m test`
- associate "application/x-shellscript" with Leafpad: `mimeo --add application/x-shellscript leafpad.desktop`
- Associate all text files with Medit: `mimeo --add 'glob:text/*' medit.desktop`
- Association File Examples: (mimeo --assoc-help)

```
vlc --one-instance --playlist-enqueue %U
    ^https?://(www.)?youtube.com/watch\?.*v=

Open HTTP(S) URLs with Firefox:

/usr/bin/firefox %U   
    ^https?://

Open various media files in VLC by extension:

/usr/bin/vlc --one-instance --playlist-enqueue %F
  \.mp3$
  \.flac$
  \.avi$
```

- CUSTOM ASSOCIATION FILES (mimeo --help, mimeo --filepath-help
If --assoc is not passed then the following paths will be checked for custom associations, in order:

```bash
/home/goncalo/.config/mimeo/associations.txt
/etc/xdg/mimeo/associations.txt
```

Note: Eventually try mimi! Links:
- [repo](https://github.com/taylorchu/mimi)
- [aur](https://aur.archlinux.org/packages.php?ID=56438	)

Note: eventually take a look at package perl-file-mimeinfo (mimeopen -d )

<div style="page-break-after: always; break-after: page;"></div>

# 21. Color-Scheme

- Install: python-pywal
- Install: `yay -S fzwal-git`
- Run: `wal --theme base16-nord`
- Add to .zshrc: (`cat ~/.cache/wal/sequences &`)
- Add to .vimrc:
  - Plug 'dylanaraps/wal.vim' (install with PlugInstall)
  - `colorscheme wal`
  - `set background=dark`

NOTE:

- This pywal thing seems to screw up with other windows. Removed for now!
- It seems like it isn't pywal that messed with firefox -> Firefox stopped crahsing when I disabled the popOS gtk theme!!!

<div style="page-break-after: always; break-after: page;"></div>

# 22. LibreOffice

- Latex in impress: `pacman -S libreoffice-extension-texmaths`
- Check extension in Extension Manager inside libreoffice
- To install ExpandAnimations go to Tools->ExtensionManager and add there the oxt file

<div style="page-break-after: always; break-after: page;"></div>

# 23. Reflector

```bash
reflector --latest 200 --protocol http --protocol https --sort rate --save /etc/pacman.d/mirrorlist
reflector --country 'France,Germany' --age 12 --protocol https --sort rate --save /etc/pacman.d/mirrorlist
```

<div style="page-break-after: always; break-after: page;"></div>

# 24. AceStream

```bash
yay -S acestream-engine
yay -S acestream-launcher
acestreamid
acestream-launcher acestream://id -p player 
```

<div style="page-break-after: always; break-after: page;"></div>

# 25. Swig

```bash
g++ -Wall -Wextra -Wpedantic -I/usr/include/python3.9 -I/usr/lib/python3.9/site-packages/numpy/core/include/ -fPIC -shared example_wrap.cxx -o _example.so -lpython3.9   
the first includes python and the second numpy/arrayobject.h
```

<div style="page-break-after: always; break-after: page;"></div>

# 26. TTY Login

## 26.1. Add Username

```bash
cat /etc/systemd/system/getty@tty1.service.d/override.conf:
  [Service]
  ExecStart=
  ExecStart=-/usr/bin/agetty -n -o <username> %I
systemctl edit getty@tty1
```

## 26.2. Change startup message

1) added script to bin folder that re-writes /etc/issue with the correct value of the  baterry. It uses a template situated in issue folder. This template has a PLACEHOLDER  text that is used by sed to substitute with the value of the battery. In order for this to work, I created a systemd service (check systemd_scripts folder) which runs the 
script. Everything is situated in lap_dotfiles

<div style="page-break-after: always; break-after: page;"></div>

# 27. HPC

## 27.1. Modules

- To list all currently loaded modules: `module list`
- To list all available (loadable) modules: `module avail`
- To load a module: `module load x`
- To unload a module: `module unload x`
- To swap a specific module for another: `module switch x y`

## 27.2. Some Commands

```bash
sinfo
squeue
scontrol show partition/node/....
scancel (process_id)
# Don't forget to load modules - e.g. -> module load gcc-8.1, module load openmpi/4.0.1
module avail # to see modules
srun -n 1 -p partition bash # takes me to a shell inside the node
```

Launch Script:

```bash
#!bin/bash
#SBATCH # instrucoes ao sbatch
./ficheiro.out
```

<div style="page-break-after: always; break-after: page;"></div>

# 28. Network

## 28.1. Network not connecting at startup

- `systemctl restart NetworkManager`

## 28.2. MAC address

- To find the default device -> `ip route list`
- To find the mac address -> `ifconfig -a`
- Alternatives:
  - `ip addr show && ip addr show device`
  - `ip link show`

<div style="page-break-after: always; break-after: page;"></div>

# 29. Dmenu_ext

## 29.1. Not opening paths

Add to mimeapps.list: inode/directory=pcmanfm.desktop;

<div style="page-break-after: always; break-after: page;"></div>

# 30. Nvidia

## 30.1. NVIDIA back screen on TTY

- /etc/modprobe.d/blacklist.conf:

  ```bash
  install i915 /usr/bin/false
  install intel_agp /usr/bin/false
  ```
  
<div style="page-break-after: always; break-after: page;"></div>

# 31. CFP Nvidia

## 31.1. VPN access

- Install snx from InfoCiencias
- create .snxrc file
- connect by snx
- disconnect by snx -d

## 31.2. First steps to config account

- To create home directory by default: CREATE_HOME yes in /etc/login.defs
- On first login had no home:
  - mkdir /home/username
  - chown username:username /home/username
  - cp -rT /etc/skel /home/username -> to populate with default files and folders
- Generate ssh keys: ssh-keygen
- Add .pub key to ~/.ssh/authorized_keys
- The default shell was /bin/sh. So that bash works,
  - chsh
    /bin/bash
- Can check shells by: cat /etc/shells

<div style="page-break-after: always; break-after: page;"></div>

# 32. Awk

- Print every 3 lines

  ```bash
  awk 'NR%3==0' file
  awk 'NR%3==0' file >> tmp && mv tmp file -> saving to file
  for i in ./file_pattern ; do
    awk 'NR%3==0' $i >> tmp && mv tmp $i 
  done
  # The above cycle iterates over the files in the current directory
  ```

<div style="page-break-after: always; break-after: page;"></div>

# 33. Sublime-Text

- Go to sublime text webpage, linux repos and find pacman. Follow the commands
  - Go to preferences -> package control (to install the package manager)
  - To install a package: Ctrl + Shift + p (command pallet) -> Install -> Package name
  - Imporant packages to install: (To see packges: Preferences->Package Control->List Packages)
    - SFTP
    - C++ Starting Kit
    - C++NamespaceTool
    - ClangFormat
    - Anaconda
    - C Improved
    - C++11
    - SideBarEnhancements

- Define shorcuts for sftp: Preferences->Package Settings->SFTP->Key Bindings
 and write on the file on the right hand side with the directory:
.config/...../Packages/User/...
My first shortcuts were: alt+z(open files) e alt+x(open servers)

- Example file for server setup:

  ```text
  {
    // The tab key will cycle through the settings when first created
    // Visit https://codexns.io/products/sftp_for_subime/settings for help

    // sftp, ftp or ftps
    "type": "sftp",

    "sync_down_on_open": true,
    "sync_same_age": true,

    "host": "176.79.187.130",
    "user": "goncalo",
    //"password": "",
    //"port": "22",

    "remote_path": "/home/goncalo/Documents/Optics/NonLinearOptics_Interpolation/",
    //"file_permissions": "664",
    //"dir_permissions": "775",

    //"extra_list_connections": 0,

    "connect_timeout": 30,
    //"keepalive": 120,
    //"ftp_passive_mode": true,
    //"ftp_obey_passive_host": false,
    //"ssh_key_file": "~/.ssh/id_rsa",
    //"sftp_flags": ["-F", "/path/to/ssh_config"],

    //"preserve_modification_times": false,
    //"remote_time_offset_in_hours": 0,
    //"remote_encoding": "utf-8",
    //"remote_locale": "C",
    //"allow_config_upload": false,
  }
  ```

- To use clang on save:
  - Install clang (pacman -S clang) and the clang package in sublime
  - Preferences->Package Settings->Clang Format->Setting-User:

    ```text
    {
      "binary": "/usr/bin/clang-format-3.8" (/path/to/your/clang-format/executable/file),
      "format_on_save": true,
      "style": "Custom",
    }
    ```

  - Preferences->Package Settings->Clang Format->Custom Style-User:

    ```text
    {
      "Language": "Cpp",
      "TabWidth": 4,
      "AlignTrailingComments": "true",
      "UseTab": "Never",
    }
    or 
    Language: Cpp
    BreakBeforeBraces: Attach
    PointerAlignment: Right
    TabWidth: 4
    IndentWidth: 4
    AccessModifierOffset: 0
    ColumnLimit: 120
    NamespaceIndentation: All
    AlignTrailingComments: true
    AllowAllParametersOfDeclarationOnNextLine: true
    AlwaysBreakTemplateDeclarations: true
    UseTab: Never
    ```

<div style="page-break-after: always; break-after: page;"></div>

# 34. Config-Printer

## 34.1. CUPS

- Packages to install:
  - cups, cups-filters, liblouis, qpdf, cups-pdf, python-pycups, python-pycurl, gsfonts
  - system-config-printer

- Services to activate

  ```bash
  sudo systemctl enable --now cups.service
  sudo systemctl enable --now cups.socket
  sudo systemctl enable --now cups.path
  ```

- List services:
  `sudo systemctl -a list-units | grep -i cups`
- Configuration:
  - Verify the following user groups are set in file /etc/cups/cups-files.conf
  `SystemGroup sys root wheel`
  - Associate a user to the "sys" group by replacing "username" below:
  `gpasswd -a username sys`

- Add A Printer Using CUPS Web Interface
  - Open "Manage Printing" or browse to http://localhost:631/
  - Click on “Administration” at the top of the web page.
  - Click on “Add Printers”.
  - Select the desired printer under "Discovered Network Printers" and click the "Continue" button.
  - Set the "Name", "Description" and "Location" and then clock on the "Continue" button.
  - Select the "Model" of printer and click the "Add Printer" button.
  - Select default options and click the "Set Default Options" button.
- Add A Printer Using Printer Settings
This utilizes "Printer Settings" (system-config-printer package) a native GUI application.
  - Open "Printer Settings".
  - Click on the "Unlock" button.
  - Click on the "Add" button.
  - Select the desired printer and click the "Forward" button.
  - Set the desired "Printer Name", "Description" and "Location".
  - Click the "Apply" button.

After these steps, it should work. Do not need to go for avahi!!!!

## 34.2. AVAHI

- Packages to install:
  - avahi, nss-mdns
- `sudo systemctl enable avahi-daemon.service`
- edit the file /etc/nsswitch.conf and change the hosts line to include
`mdns_minimal [NOTFOUND=return]`
before the word resolve
- avahi-browse --all --ignore-local --resolve --terminate
or
- avahi-discover (needs gtk3, dbus-python and python-gobject)

The question is not avahi or cups but : Do I need/want printer autodiscovery or not ?
If answer is yes > enable avahi , if answer is no > disable avahi
Either use cups or cups + avahi

## 34.3. HP SCANNER

- wiki page: SANE/Scanner-specific problems
- pacman -S sane-airscan ipp-usb
- pacman -S hplip
- Go to system-config-printer and now add printer (printing should work from now on).
  In order to scan:
  - `hp-makeuri <scanner_ip> / scanimage -L`
  - `scanimage --device "<hpaio:/net....>" --format=png --resolution 300 >scan.png`

<div style="page-break-after: always; break-after: page;"></div>

# 35. Sway

## 35.1. Packages to check for base arch install

```bash
pacman -S grub efibootmgr networkmanager network-manager-applet dialog wpa_supplicant mtools dosfstools reflector base-devel linux-headers avahi xdg-user-dirs xdg-utils gvfs gvfs-smb nfs-utils inetutils dnsutils bluez bluez-utils cups hplip alsa-utils bash-completion openssh rsync reflector acpi acpi_call tlp virt-manager qemu qemu-arch-extra edk2-ovmf bridge-utils dnsmasq vde2 openbsd-netcat iptables-nft ipset firewalld flatpak sof-firmware nss-mdns acpid os-prober ntfs-3g terminus-font
pacman -S xdg-desktop-portal-wlr
```

## 35.2. Services

```bash
systemctl enable NetworkManager
systemctl enable bluetooth
systemctl enable cups.service
systemctl enable sshd
systemctl enable avahi-daemon
systemctl enable tlp # You can comment this command out if you didn't install tlp, see above
systemctl enable reflector.timer
systemctl enable fstrim.timer
systemctl enable libvirtd
systemctl enable firewalld
systemctl enable acpid
```

## 35.3. Sway install from YT:

`pacman -S sway swaylock swayidle xorg-xwayland ttf-font-awesome`

## 35.4. Sway my experience

### 35.4.1. Packages

```bash
pacman -S sway swaylock
pacman -S mako grim
yay -S grimshot
pacman -S wl-clipboard
pacman -S light (manage brightness)
pacman -S playerctl (waybar config)
pacman -S waybar
yay -S swaylock-effects-git
pacman -S swayidle
pacman -S xdg-desktop-portal-wlr
pacman -S dex
yay -S rambox-bin
yay -S albert-minimal
pacman -S pamixer
pacman -S brightnessctl
yay -S nordic-theme
yay -S clipman
# installed i3-quickterm from github: https://github.com/lbonn/i3-quickterm.git
```

### 35.4.2. Configuration

- The first config lines are concerned with environment variables needed to make gtk applications launch faster:
  - exec systemctl --user import-environment DISPLAY WAYLAND_DISPLAY SWAYSOCK
  -	exec hash dbus-update-activation-environment 2>/dev/null && \
  dbus-update-activation-environment --systemd DISPLAY WAYLAND_DISPLAY SWAYSOCK
- The keyboard and touchpad are configured in sway config. To get the inputs run: swaymsg -t get_inputs
- using i3-quickterm to have a dropdown menu. Need to install rofi for it to work but I can also use i3-quickterm shell and then I do not need to install rofi.
- binding albert in config with exec albert toggle
- using swaylock-effects-git for sway lock
- Using "exec grimshot copy area" for screenshots (requires wl-clipboard) 
- Bind media keys (brightness and volume) on config. Associated icons to notifications. The icons are from Arc-X-D package.
- If I want to use light, need to add the following line to sudoers: %wheel ALL=(root) NOPASSWD: /usr/bin/light
- Install playerctl for these controls and waybar.
- For the autostart applications, need to add the flag --indicator to nm-applet
- For the dual monitor, check the monitor with swaymsg -t get_outputs
- Sway doesn't work very well with lightdm -> use lydm -> systemctl enable ly.service -f
- Instead of using ly, simply use .zprofile to login. For it to work, need whiptail and
Rebelo's package shiftstate (it is on lap_dotfiles). Ctr+Enter after putting pw on 
tty takes me to a tui to choose the wm. Shift+Enter takes me to tty login
- The env variable MOZ_ENABLE_WAYLAND=1 enables to run firefox on wayland mode. 
However, it doesn't load the gtk theme this way. Then, I added to .confi/sway/env the
flag GTK_THEME=Nordic. Need to change this in accordance to the gtk theme I want

### 35.4.3. Fix cannot open display

`pacman -S xorg-server-xwayland`

	
### 35.4.4. Mathematica

- In order to run mathematica: `QT_QPA_PLATFORM="xcb" mathematica &`
- A better way is to add a folder: $HOME/bin and the following script name mathematica
(same name as the original in /usr/local/bin):
  ```bash
  #!/bin/sh
  QT_QPA_PLATFORM="xcb" /usr/local/bin/mathematica "$@"
  ```
- Then, if in sway, add to the env script in .config/sway the following line:
	`PATH="${HOME}/bin:${PATH}"`
The fact that $HOME/bin comes before path overrides the original mathematica script!Now,
I can launch mathematica from dmenu
- Although the above steps solve the problem when we call the binary mathematica,
it doesn't solve the problem when we want to open a mathematica notebook through the
file manager. To solve that problem I need to change the wolfram-mathematica12.desktop
file in /usr/share/applications/wolfram-mathematica12.desktop. In the field exec I need
to put the path to $HOME/bin/mathematica script. I saved the original desktop file in  /usr/share/applications/mathematica.desktop.
- mathematica was crashing with 3D graphics. Solution: run mathematica with mesa: mathematica -mesa notebook_name.

### 35.4.5. Zoom

- Currently doesn't allow for sreen sharing. Use zoom in firefox and it works fine!
- Eventually try XGD_CURRENT_DESKTOP=gnome zoom

### 35.4.6. Albert

- albert crashing after search or cancelling search: rm .config/albert/core.db

<div style="page-break-after: always; break-after: page;"></div>

# 36. Rclone

## 36.1. Config

- rclone is best configured using ssh-agent:
  - rclone config
- new remote
- Storage > sftp
- host: 192.168.1.64 (e.g)
- user: goncalo (e.g)
- ssh port: blank
- To use ssh-agent, leave all the other options blank (and eventually refuse them)

## 36.2. Rclone union

```text
[paulo_http_single]
type = http
url = https://joserebelo:PASSWORD@paulo

[paulo_http]
type = union
upstreams = paulo_http_single:/:ro /cache/union
```

- The first part on the union config is read-only but `/cache/union` is not, allowing to add our own stuff
- We need to mount (for the union to work) the `[paulo_http]` one.
- what we write in the mounted drive will go to /cache/union and reading merges both

## 36.3. Problem

- NewFs: couldn't connect SSH: ssh: handshake failed: ssh: unable to authenticate, attempted methods [none publickey], no supported methods remain
- This was happening because of the type of keys. I should generate: ssh-keygen -t ed25519
- Solution: add to /etc/ssh/sshd_config: PubkeyAcceptedAlgorithms=+ssh-rsa
- I should also add:
  
  ```text
  PermitRootLogin no
  PasswordAuthentication no
  ```

## 36.4. Sync

- `rclone sync /home/goncalo/Documents pi:/home/goncalo/HDD/Documents/Backups/Laptop/Documents --log-file /home/goncalo/.local/my_logs/backup.log -v --exclude lap_dotfiles/ --transfers=8 --progress`
- -i flag asks question about copying 

## 36.5. OneDrive

- `rclone copy UsefulScripts OneDrive:Documents/UsefulScripts` (copies the contents of UsefulScripts -> therefore I copy to Documents/UsefulScripts, otherwise would populate Documents with its contents)

<div style="page-break-after: always; break-after: page;"></div>

# 37. Pipewire

- `pacman -S pipewire`
- `pacman -S pipewire-pulse`. Remove pulseaudio and pulseaudio-bluetooth
- It automatically creates symlink `/etc/systemd/user/sockets.target.wants/pipewire-pulse.socket → /usr/lib/systemd/user/pipewire-pulse.socket`
- Disable pulseaudio on sway config
- `pacman -S libpulse` (comes with pulseaudio)
- `pacman -Qo pactl`
- bluetooth should not be affected by this
- pacmd used by volume-script no longer works. Need to use amixer (which comes with alsa-utils) to check if muted or not.

<div style="page-break-after: always; break-after: page;"></div>

# 38. Fail2Ban

- `pacman -S fail2ban`
- enable/start fail2ban.service

## 38.1. Configuration
Edit file /etc/fail2ban/jail.local:

```text
[DEFAULT]
bantime = -1
findtime = 1d
maxretry = 5

[sshd]
enabled = true
```

<div style="page-break-after: always; break-after: page;"></div>

# 39. Systemd-User

- Can configure `/etc/systemd/user.conf` and set the default environment for the units. Affects all user units:

```text
[Manager]
DefaultEnvironment="PATH=/usr/local/sbin:/usr/local/bin:/usr/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl:/opt/vc/bin:/home/goncalo/.local/bin"

DefaultEnvironment="VAR1=word1 word2" VAR2=word3 "VAR3=word 5 6" -> Sets three variables "VAR1", "VAR2", "VAR3".
```

- `systemctl status <name>.service` to show the status of a given service. The PID is also shown. `sudo strings /proc/<PID>/environ` allows to look at the actual environment of the process.
- For services of `Type=oneshot`, the behavior is similar to simple - but the service manager will consider the unit up after the main process exits. `oneshot` can be used with `RemainAfterExit`. For the case of the while loop, I do not want any of these, since if the script exits, then it means it finished. With `Type=oneshot`, the `systemctl --start` command left hanging.
- Useful link [stack overflow](https://stackoverflow.com/questions/39032100/what-is-the-difference-between-systemds-oneshot-and-simple-service-types).

<div style="page-break-after: always; break-after: page;"></div>

# 40. Systemd-Resolved

`/etc/systemd/resolved.conf`:

```text
[Resolve]
DNS=1.1.1.1#cloudflare-dns.com 9.9.9.9#dns.quad9.net
FallbackDNS=1.0.0.1#cloudflare-dns.com 9.9.9.10#dns.quad9.net
DNSSEC=yes
DNSOverTLS=yes
Cache=yes
CacheFromLocalhost=no
DNSStubListener=yes
ReadEtcHosts=yes
```

`/etc/resolv.conf`:

`ln -rsf /run/systemd/resolve/stub-resolv.conf /etc/resolv.conf`

`/etc/NetworkManager/NetworkManager.conf`:

```text
[main]
# Ignore network-provided dns
dns = none
```

## 40.1. Activate Service:
`systemctl enable systemd-resolved.service`

## 40.2. systemd-networkd

I can force the dns of a given interface like this:

```text
Edit sudo cat /etc/systemd/network/vpn.network

[Match]
Name=vpn*

[Network]
DHCP=yes
DNS=10.0.1.2
Domains=~critical.pt
```

where `Name` needs to match the name of the interface.

Then, simply: `systemctl start systemd-networkd`.

<div style="page-break-after: always; break-after: page;"></div>

# 41. Dual Boot

## 41.1. Windows After Linux

- Install windows;
- Boot live iso; mount disk with linux:
  - `mount /dev/sdX2 /mnt`
  - `mount /dev/sdX1 /mnt/boot/efi`
  - `manjaro-chroot /mnt`
  - `update-grub`
- If windows keeps changing boot entry order:
  - Install EasyUefi (easyuefi.com)
    - Go to Manage EFI boot option
  - Check the path to the manjaro boot option
  - `Bcdedit /set {bootmgr} path path\from\above\step` (e.g. \EFI\Manjaro\grubx64.efi)

## 41.2. Fix Windows bootloader Gone

- shift+f10
- diskpart
- list disk
- select disk X (Where windows was installed)
- list volume
- select volume Y
- assign letter=Z (where Z is the letter you want to "mount")
- do the same to efi partition:
  - list disk
  - select disk X (Where is the EFI partition)
  - list volume
  - select volume volume-number
  - assign letter=M 
- exit diskpart (exit)
- run: `bcdboot <Letter-Assigned-To-Windows>:\Windows`
  eg: bcdboot Z:\Windows
  - optionally: `bcdboot Z:\Windows /s M:` (/s copies to drive M)
- Unmount devices:
  - diskpart
  - list volume
  - select volume VOLUME-NUMBER
  - remove letter DRIVE_LETTER

<div style="page-break-after: always; break-after: page;"></div>

# 42. RP Monitor

- for the monotoring need 3 docker containers: grafana, influxdb (database), telegraf
  - the ports on docker-compose need to match the ones in telegraf.conf
  - In the telegraf conf:
    - urls: needs to be 127.0.0.1:(port of docker compose)
    - username and pw must match what I put in influxdb
    - hostname must be the one on of pi

## 42.1. Create db in influxdb

```bash
docker exec -it influxdb bash 
influx
CREATE USER "grafana" WITH PASSWORD 'qwe' (pw configured in grafana)
CREATE USER "telegraf" WITH PASSWORD 'asd' (pw put on config)
CREATE DATABASE "pi"
GRANT ALL ON "pi" TO "grafana"
GRANT ALL ON "pi" TO "telegraf"
SHOW DATABASES
```

## 42.2. CONFIG GRAFANA

- add data source:
  - Configuration -> Data Sources:
  - url: http://influxdb:8086
  - database: pi
  - User: grafana (same as defined in influxdb)
  - Pw: same as defined in influxdb
- import dashboard:
  - ID: 10578
  - Select data source added above

## 42.3. Notes

- In order to restart a container do docker-compose up container_name (this reloads the yml if it changed); otherwise use docker-compose restart container_name
- `docker rm -f container_name` (deletes container)
- `docker inspect influxdb | jq ".[0].Config.Volumes"`
- In telegram.conf I need 127.0.0.1 : nas portas means "bind to all addresses" mas aqui quero mesmo aceder ao localhost

<div style="page-break-after: always; break-after: page;"></div>

# 43. Docker

- `pacman -S docker docker-compose`
- `systemctl enble docker.service`
- docker info; `sudo chmod 666 /var/run/docker.sock`
- On folder, run: `docker-compose up -d`
- To access things on the web, check the port on .yml file and: http://localhost:8080
- To access using any device on the network, substitute 127.0.0.1 to 0.0.0.0 in all containers in the .yml file
  Then, only need to do ip(192.168.1.64):port on any device and it will work.
- Login on web: admin, pw: adminadmin
- On qbittorrent, tools->options->default save path: /downloads/

  Notes on the downloads folder:
  - It is important that this folder is mounted to some directory on my computer (check docker-compose) and that this mount point is the same in radarr/sonarr. Radarr/sonarr will check the download folder in the qbittorrent settings (which is /downloads) and will therefore look in the directory /downloads. Therefore, /downloads must be a volume in docker-compose and should point to the same folder as in qbittorrent.
- On qbittorrent, tools->options->(under automatically add torrents from) Monitored Folder -> /blackhole
- Get image: https://hub.docker.com/r/linuxserver/radarr
- `docker ps -a` -> check running containers
- To set pw and username on qbittorrent: Tools -> Options -> Connection -> Authentication
- Rebuild image: docker-compose build rclone-extension --no-cache

## 43.1. Jacket

- http://localhost:9117
- Add indexer -> RARBG and 1337x;

## 43.2. Sonarr

- Download clients -> Clicl + -> Select qbittorrent -> host é qbittorrent (you can access containers by name)
- Port: 8080
- Username and Pw : same as qbittorrent login (admin, adminadmin)
- We can access a container from the terminal: docker exec -it qbittorrent bash
- Go to Indexers -> Select Torznab -> In URL paste the Torznab feed from jackett (and change localhost to jackett in the URL)
- Add API key from jackett (on top of the page)
- If this doesn't work, change dns:
  - `vim /etc/resolv.conf`
  - `nameserver 1.1.1.2`
- vim /etc/NetworkManager/NetworkManager.conf
  
  ```text
  [main]
  # Ignore network-provided dns
  dns = none
  ```

- check if I can ping from jackett: `docker exec -it jackett bash; curl 1337x.to`
- `systemctl restart docker`
- `docker-compose up -d`
- When adding series, the root folder should be: /media -> this is mapped to a volume outside the container
- qbittorrent downloads to /downloads and sonarr moves it to /media
- old episodes on sonarr must be downloaded manually
- A lupa saca automatico e o boneco deixa escolher o torrent
- If I can't add indexer, I can add one that I know that works and then edit it and substitute the url for the one I want to add.
- Add series on read-only file system:
  - Mount read-only fs inside container
  - Add new series to default path where sonarr can write
  - Open sqlitebrowser -> Open Database -> sonardb (inside config folder in container) -> In table, select Series -> find series -> Select Path -> Change on the right

### 43.2.1. Add manually downloaded season

- Go to Wanted on the meny on the left
- Manual Import
- Select Folder with manually downloaded season
- Move automatically

## 43.3. System service to run docker

  ```text
  /etc/systemd/system/docker-compose.service

  [Unit]
  Description=Docker Compose Service
  Requires=docker.service
  After=docker.service
  After=network-online.target
  Wants=network-online.target

  [Service]
  Type=oneshot
  RemainAfterExit=yes
  WorkingDirectory=/home/jose/dotfiles/pi
  ExecStart=/usr/sbin/docker-compose up -d
  ExecStop=/usr/sbin/docker-compose down
  TimeoutStartSec=0

  [Install]
  WantedBy=multi-user.target
  ```

## 43.4. Rclone DLNA

- Settings -> Download clients -> Advanced options -> Enable remove imported downloads from download client history
- This is streaming the /media folder to my network
- In VLC go to view -> playlist -> local network -> universal plug and play

## 43.5. Transdrone

Description: App for android to manage torrents

## 43.6. JellyFin

- drive ntfs -> does not support inotify -> scan manually: Settings -> dashboard -> scan all libraries
- In order to change folder go to settings -> Dashboard -> Libraries
- If informations are not correct, select movie or series and click identify
- Do not watch jellyfin on browser. Instead, yay -S jellyfin-media-player

- DNLA
  - add to yml: "network_mode: host" on jellyfin container and remove ports section

## 43.7. QBitTorrent

- In order to stop seeding go to tools -> bittorrent -> seeding limits -> min ratio 0.01 -> max seed time 1 minute (Pause torrent, remove doesnt work)

## 43.8. Bazarr

- Go to settings -> Languages -> Add New Profile -> Add desired languages -> Below this option, check the boxes Series and Movies and choose the profile just created in the step before

## 43.9. Organizrr

- In order for qbittorrent to work: Tools -> WebUI -> Untick "Enable clickjacking protection" and "Enable Cross-Site Request Forgery protection"

## 43.10. NginX

- Need to get nginx.conf and proxy.conf from swag github;
- On the nginx.conf carefull with the following lines:
  - include /config/nginx/worker_processes.conf;
  - include /config/nginx/resolver.conf;
- /config/nginx/resolver.conf:
  - `resolver  127.0.0.11 valid=30s;` (note that the ";" is important in these files
- The configs to reverse proxy can be found in github: linuxserver/reverse-proxy-confs (I want the subfolder ones)
- In order to setup the sonarr, jackett, etc reverse-proxy config, I need to read the config because it asks to change the Base URL, etc
- In order to setup grafana, needed to add to the docker-compose config:
  - environment:
    - "GF_SERVER_ROOT_URL=%(protocol)s://%(domain)s:%(http_port)s/grafana/"
- The above configs only have the "location" block which goes inside the server block. The default server config can be found in /config/nginx/site-confs/default. There, I should add "include /config/nginx/proxy-confs/.*subfolder.conf;" and comment both "location" blocks there.
- The organizr config has as upstream_port port 80. In docker-compose.yml, organizr has host post 9983 mapped to port 80 on the container. However, nginx bypasses that and goes straight to port 80 on the container -> that's why the reverse proxy config works.
- It happened that, when I connected to organizr behind the nginx server, I could not login. This happened because the browser was rejecting cookies. The problem was in proxy.conf file. It assumed it was in https. Only need to comment the lines:
  - `proxy_set_header X-Forwarded-Proto https;`
  - `proxy_set_header X-Forwarded-Ssl on;`

- Changed all port mapping in docker-compose.yml to 127.0.0.1:port so it can only be access from pi. Since everything is reverse proxied, it's fine
- The nginx docker-compose config has in port section:
  - 80:80 which defaults to 0.0.0.0:80:80 (that's why I can access nginx from the entire network)
- In order to reverse-proxy emby I commented out the line "network_mode: host" otherwise the reverse-proxy config does not work by default. If I want to use "network_mode: host" I need change the reverse-proxy config: "set $upstream_app emby" -> "set $upstream_app 10.0.10.1". Inside emby, in Network, need to change "Secure connection mode" to "Handled by reverse proxy". One thing I noticed was that UPnP was not working. In order for it to work, in emby, I need to add, in Network -> Lan Networks: 192.168.0.0/24, 10.0.10.0/24  

- Couldn't find rclone serve dlna in laptop with firewalld. Use firewall gui, go to options -> change zones of connections -> select my network and put it as home. Then, select my network in connections, in zones tab  select home, then services, and tick upnp-client

- In the media reverse proxy config, the lines: "alias /media" and "facyindex on" are the ones responsible to show the content of the folder /media of the container (folder where I wanna mount the stuff I wanna show). Note that I also need to "git clone https://github.com/alehaa/nginx-fancyindex-flat-theme.git" and
  
  ```text
  sed -i '/<small>/,/<\/small>/d' "$FANCYINDEX_THEME_PATH/layout/footer.html"
  sed -i "s/File Browser/$(cat /etc/hostname) \| media/g" -i "$FANCYINDEX_THEME_PATH/layout/header.html"
  sed -i "s/'Home'/''/g" -i "$FANCYINDEX_THEME_PATH/layout/js/breadcrumbs.js"
  ```

## 43.11. Some Important Concepts

- Docker bypasses iptables
- localhost de um container não é o mesmo que de outro (estao isolados)
- Can't specify ports with network_mode host
- In iptables.rules, the line:
  `":FORWARD DROP [0:0]"`

  blocks all forwarded packets
- If I want to find the docker ip of a container: `docker network inspect -f '{{range .IPAM.Config}}{{.Subnet}}{{end}}' <container_id>`
- The `<container_id>` can be found by running `docker ps -a`
- `docker inspect <container_name>`
- `docker stop/logs/(rm -f)/restart <container_name>`
- `docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' <container_id>`
- `docker images -> prints images of containers`
- `docker image inspect <image_id_from_above_step>`
- `docker manifest inspect --verbose <container_name>`

## 43.12. Update Containers

- `docker-compose pull`
- `docker-compose up`

- Container to update containers

  ```text
    watchtower:
      container_name: watchtower
      image: containrrr/watchtower:latest
      networks:
        - monitoring
      volumes:
        - /var/run/docker.sock:/var/run/docker.sock
      command: >-
        --cleanup --rolling-restart --schedule "0 0 4 * * *"
  ```

Info: --cleanup doesn't leave older version on the computer.
      --rolling-restart restarts the containers one by one (important to deal with dependencies)
      The container pulls automatically

- `docker system prune -a` (after doing docker-compose up, otherwise deletes images I just pulled)
- list images: `docker images -a`
- remove all images: `docker rmi $(docker images -a -q)`

## 43.13. Some notes based on experience

- `docker run -it image_name sh` -> runs an interactive shell container using the image "image_name"
 The above command can be necessary because if the container is a one-shot, it will simply die after running: `docker run <image_name>`
 However, I can also do `docker run -t -d <image_name> sh` and, even it's an one-shot, it will be kept alive. Then, I can always do a `docker exec -it <container_id> sh` to enter again inside the container
- Other ways of starting a container: `sudo docker create <image_name>; sudo docker start <container_id_from_previous_command>`
- `docker image history --no-trunc image_name > image_history` -> steps in the Dockerfile
- `docker ps -a` -> lists containers and the container id
- save the id in a variable: `container_id=$(docker create image_name)`
- Extracting a file from an image: `docker cp "$container_id:$source_path" "$destination_path"`
- Pushing a file to an image: `docker cp folder/. "<container_id>:/path/in/container"`  -> this actually pushes all files inside folder
- `docker image inspect <image>`
- `docker container prune` -> removes all containers
- `git reset HEAD~1` -> go back one commit before pushing
- jenkins scm
- https://www.infoq.com/articles/build-a-container-golang/

<div style="page-break-after: always; break-after: page;"></div>

# 44. VPN

## 44.1. Configuration
 
- `pacman -S wireguard-tools` (wireguard-dkms, headers)
- script wgg from rebelo:
  - `WG_PEERS`: names of  the devices I want connected to the VPN
  - `NODE_URL` is the public ip
  - `WG_NODE_ADDRESS` is the desktop's ip inside the VPN
  - `WG_VPN_LAN` is the VPN network (which must match the IP chosen in the above line)
  - The `WG_NODE_INTERFACE` can be seen running: ip addr show
  - The script may be run again in order to add devices (the configurations before won't be altered)
- Open port on router:
  - Go to games and apps, configuration, and remove all the ports there;
  - Protocol: UDP
  - Log and CONE unchecked (like everything else really)
  - Port: 57278
- In order to show a qrcode for the wireguard app on cell phone: qrencode -t ansiutf8 -r /etc/wireguard/peers/telemovel.conf
- Give wireguard on cellphone root privileges
- On phone's wireguard, tunnel name can be anything I want

- To turn vpn on: `sudo wg-quick up wg1`
- Startup: `sudo systemctl enable wg-quick@wg1`
- To check hand shakes: `sudo wg show wg1 latest-handshakes`
- In order to fix the problem of the VPN not starting with systemctl service, a possible cause might be fail2ban. Then:
  - vim `/usr/lib/systemd/system/fail2ban.service`
  Append to "After= :" the following: wg-quick@wg1.service
- On laptop: `pacman -S wireguard-tools`
- Copy `/etc/wireguard/peers/laptop.conf` to `/etc/wireguard/wg0.conf`
- `sudo wg-quick up wg0`
- ip r show show the routes

## 44.2. Notes

- Each computer needs an individual ip and key
- For example, if I copy my laptop's file and put it in another computer, changing the ip, it won't
work if both connect since the key is the same
- IPS have 32 bits
- With A.B.C.D/X we mean that the X most significant digits are considered: 192.168.1.0/24 -> 192.168.0.x with x between 0 to 255
- 192.168.0.0/16 -> 192.168.0.0 to 192.168.255.255

## 44.3. Viseu

- na config do desktop do porto, tens lá uma entrada para cada peer
- no peer de viseu, para alem de 10.0.10.4/32, adicionavas 192.168.20.0/24
- e nos peer/*.conf também
- ou seja, de qualquer lado, o teu telemóvel sabia que, para chegar à rede 192.168.20.0/24, tem que enviar pacotes para o desktop do porto
- e o desktop do porto sabe que, para chegar a essa mesma rede, tem que enviar pacotes para o peer de viseu
- tinhas que adicionar a 192.168.20.0/24 no peer de viseu em wg1 no desktop do porto
- e nos peers tinha de adicionar  192.168.20.0/24 para cada um dos peers saber que, pelo desktop do porto, consegue chegar a viseu

## 44.4. Check Ports

- sudo nmap -sU -p- ip (UDP)
- sudo nmap -sT -p- ip (TCP)

## 44.5. Fix connection problem

- On laptop:
  - ip route add 192.168.1.64/32 via 192.168.1.254 dev (interface, ex: wlp0s20f3)
  - nmcli connection show
  - nmcli connection modify CONNECTION_NAME (ex: ROBOREDO) +ipv4.routes "192.168.1.0/24 192.168.1.254"
- Apparently, this fix isn't permanent

## 44.6. Connect to Rebelo

- Add wg2.conf in /etc/wireguard (note: can have both vpns up)
- Alternatively, I can add the `[Peer]` section to wg1 and, then, I don't need wg2 and this works best.

- Some notes if I didn't include the `[Peer]` section inside wg1:
  - When I added the AllowedIPs on phone, I couldn't connect to Rebelo-pi. This happened because the reply from Rebelo wasn't being forwarded to phone. I would need to add something like: `iptables -A FORWARD -i wg2 -o wg1 -j ACCEPT` in wg1 config.
  - `sudo iptables -A FORWARD -j ACCEPT` also makes it work (this allows all trafic)
  - `sudo iptables -D FORWARD -j ACCEPT` reverts the above command

- Add 10.0.1.0/24 in AllowedIPs of peers
- `wg show wg1 latest-handshakes` -> to check if connection is successful
- `echo "your_private_key" | wg pubkey` -> generates public key using private key
- This connection only works when connected to vpn, even if I'm on my LAN!!!
- `tcpdump -i any icmp` (icmp are the type of packages, the ones used by ping command. This command listens to packages being sent through
my computer)

## 44.7. Allow access to my VPN on another VPN

- Create another peer. In the allowed IPs of this peer in the config of my server, it should be:

  ```text
  AllowedIPs = <IP on my network>/32, <IPs on the other network, for e.g., 10.0.20.0>/24  
  ```

  What this means is that, on my network, the traffic for this peer can come from these different ips.

- On the server config of the other VPN, they should add the `[PEER]` section of the config that I provided them. Also, their peers need to have in the `Allowed IPs` the range of IPs of my network.

  What this means is that, when they try to connect to my VPN from one of their peers, the IPs of my network are in the config of their VPN. Then, their server has a route for my VPN through the `[PEER]` section provided on the config of their server. However, since now it's their server connecting to mine, I need the public key of the server and not the public key associated with the config that I gave them. For this reason, read last point.
- Finally, I need to change the public key of the peer that I created for them and put the public key of their server.

## 44.8. UDP2RAW

- `pacman -S udp2raw-tunnel`
- Open tcp port on router for udp2raw (e.g: 58374)
- I can still have a direct port for wireguard (e.g. 57278). This is also the ListenPort in wg1.conf
- On server, run: `udp2raw -s -l "0.0.0.0:58374" -r "127.0.0.1:57278" -k "tgbyhnrfv" --raw-mode faketcp -a` :
  - "0.0.0.0:58374" -> this means traffic can come from anywhere (0.0.0.0) and udp2raw listens on port 58374, which I specifically openned in router
  - "127.0.0.1:57278" -> this means that traffic coming from port 58374 is going to be sent to port 57278, which is wireguard's port
  - Example udp2raw.service:
  
  ```text
  [Unit]
  Description=udp2raw-tunnel client service
  ConditionFileIsExecutable=/usr/bin/udp2raw
  After=network-online.target

  [Service]
  Type=simple
  RemainAfterExit=yes
  ExecStart=/usr/bin/udp2raw -s -l "0.0.0.0:58374" -r "127.0.0.1:57278" -k "tgbyhnrfv" --raw-mode faketcp -a
  Restart=on-failure

  [Install]
  WantedBy=multi-user.target
  ```

- On client: `sudo udp2raw -c -l "127.0.0.1:5634" -r "$(ssh goncalo@jgroboredo.ddns.net 'curl -s ifconfig.me'):58374" -k "tgbyhnrfv" --raw-mode faketcp -a`
  - "127.0.0.1:5634" -> local traffic to port 5634
  - "$(ssh goncalo@jgroboredo.ddns.net 'curl -s ifconfig.me'):58374" -> target is my ipv4 ip and the port where upd2raw is listening on server, meaning in this case 58374
- The only thing left is to change wireguard config in the client:
  - For this, simply create a new config;
  - Add in the `[Interface]` group the line: "MTU = 1300" (udp2raw doesn't support large packages)
  - Change endpoint to: "127.0.0.1:5634"

## 44.9. Updated VPN

- In iptables, drop all connections except the ones I want to keep;
- These connections are only concerned with the direct access to the raspberry and not the traffic thourgh vpn;
- If I want to have a peer with full access to vpn and another with restricted access (this access refers to forwarding traffic through vpn),
and I want to be able to access the restricted access peer, I need to include in the iptables.rules the following lines:
  - `-A FORWARD -m state --state RELATED,ESTABLISHED -j ACCEPT`
  Basically, the idea is that, the restricted access peer needs to send packets saying the connection is established, for example. Therefore, these packets need to be forward by the vpn... However, this peer isn't allowed to do that by default. However, this rule allows for RELATED packets to be forwarded. The similar rule existent in the wg config isn't enough probably because the packets don't go through eth0. The rule
  - `-A FORWARD -p icmp --icmp-type echo-request -j ACCEPT` allows for pings.
  - Lastly, on iptables.rules, I need to specifically allow access to each port I want to access, EVEN if I'm already connected to the vpn. The idea seems to be that
  I have access to the VPN through the VPN port, but this doesn't give me access to the other ports.

  - A container that hasn't network_mode host can't now connect to one that is on the network_mode host. To solve this, allow input from docker interface:
    - `-A INPUT -i br+ -p TCP --dport 32400 -j ACCEPT`

## 44.10. Fixing routes

- When laptop is not connected to VPN but desktop is (both in porto), I could not ping desktop from laptop using the local ip, since the wireguard
 priority was lower and the response of the desktop went through the vpn (and laptop was not connected)
- changing priorities correctly:
  - `sudo ifmetric wlp0s20f3 0`
  - `sudo ip route del default`
  - `sudo ip route add default via 192.168.200.254 dev wlp0s20f3 proto dhcp src 192.168.200.67 metric 600`
  - `sudo ifmetric wg0 1`

 NOTE:  [Nginx Server](https://hub.docker.com/r/linuxserver/swag)

## 44.11. Rebelo's Jellyfin

I need to foward the traffic in order for a peer to have access to Rebelo's Jellyfin. If the peer has full access, everything will work. If the peer has limited access and I want to maintain it like that, I need to add the following lines:

```text
PostUp   = iptables -A FORWARD -i %i -s 10.0.10.5 -d 10.0.0.0/24 -p tcp --dport 80  -j ACCEPT
PostDown = iptables -D FORWARD -i %i -s 10.0.10.5 -d 10.0.0.0/24 -p tcp --dport 80  -j ACCEPT
PostUp   = iptables -A FORWARD -i %i -s 10.0.10.5 -d 10.0.0.0/24 -p tcp --dport 443  -j ACCEPT
PostDown = iptables -D FORWARD -i %i -s 10.0.10.5 -d 10.0.0.0/24 -p tcp --dport 443  -j ACCEPT

PostUp   = iptables -A FORWARD -i %i -s 10.0.10.5 -d 10.0.1.0/24 -p tcp --dport 80  -j ACCEPT
PostDown = iptables -D FORWARD -i %i -s 10.0.10.5 -d 10.0.1.0/24 -p tcp --dport 80  -j ACCEPT
PostUp   = iptables -A FORWARD -i %i -s 10.0.10.5 -d 10.0.1.0/24 -p tcp --dport 443  -j ACCEPT
PostDown = iptables -D FORWARD -i %i -s 10.0.10.5 -d 10.0.1.0/24 -p tcp --dport 443  -j ACCEPT
```

Note: the `-d <ip>` only affects traffic that goes specifically to that ip. I am basically saying: allow fowarding to that destination.

<div style="page-break-after: always; break-after: page;"></div>

# 45. DDNS

ON ROUTER:

- Go to dynamic ddns;
- Configure -> Activate -> Username: email of no-ip account -> Password: pw of no-ip account;
 Service: No-IP -> Host: hostname chosen in no-ip account (--.ddns.net)
- Do not forget to change router's account pw to something different from default (currently, it is my usual pw)

<div style="page-break-after: always; break-after: page;"></div>

# 46. Encrypt dir

- tar -cvzf - folder | gpg -c > folder.tar.gz.gpg
  - gpg -d folder.tar.gz.gpg | tar -xvzf -

## 46.1. Disable password cache

- Edit `~/.gnupg/gpg-agent.conf`

  ```text
    default-cache-ttl 1
    max-cache-ttl 1
  ```

<div style="page-break-after: always; break-after: page;"></div>

# 47. Violent Monkey

- https://addons.mozilla.org/en-US/firefox/addon/violentmonkey/
- https://github.com/Purfview/IMDb-Scout-Mod
  - Go to script in github, raw -> ViolentMonkey will prompt to install
  - Go to imdb page of some movie/show, violentmonkey IMDB scout mod settings, search for sonnar and radarr and set it up (the root folder is the folder inside radarr and sonarr where I keep movies/tvshows).
  - Don't forget to enable them at the very end of the file
- https://greasyfork.org/en/scripts/789-select-text-inside-a-link-like-opera
- https://greasyfork.org/en/scripts/1810-google-tracking-b-gone

- Tampermonkey allows method GM_cookie

<div style="page-break-after: always; break-after: page;"></div>

# 48. Wireshark

- Dissectors: .local/lib/wireshark/plugins
- For rfcomm dlci: file -> export -> export as json

<div style="page-break-after: always; break-after: page;"></div>

# 49. Telegram

## 49.1. BotFather

```text
/newbot
BotName
botusername_bot
/setuserpic
@botusername_bot (note: this doesn't work without the "@")
```

## 49.2. Find bot chat ID

- On telegram, search by: @botusername_bot
- `https://api.telegram.org/bot<bot_token_here>/getUpdates`
- Send message to bot in telegram and update this page
- Another option is to add @RawDataBot to my group (do not forget to kick it after)

## 49.3. Add sonarr and radarr to telegram

- Go to settings -> Connect -> Telegram
- In name, just put Telegram
- Add bot token and chat id

<div style="page-break-after: always; break-after: page;"></div>

# 50. Barrier

Connect first with barrier only after do this:

- Edit `sudo vim /etc/systemd/system/barrier.service`

```text
[Unit]
Description=Barrier Client mouse/keyboard share
Requires=display-manager.service
After=display-manager.service
StartLimitIntervalSec=0

[Service]
Type=forking
ExecStart=/usr/bin/barrierc --no-restart --name raspberrypi (name I want for the client to be known) --enable-crypto 192.168.0.109 (ip of server)
Restart=always
RestartSec=10
User=pi

[Install]
WantedBy=multi-user.target
```

And do:

```bash
sudo systemctl daemon-reload
systemctl start barrier.service
systemctl status barrier.service
systemctl enable barrier.service
```

so that the service doesn't run when I go to openbox, since I want to play cs, add to /etc/sudoers : `goncalo ALL = NOPASSWD: /bin/systemctl stop barrier.service`
and add `sudo systemctl stop barrier.service` to autostart

Barrier does not work on wayland

<div style="page-break-after: always; break-after: page;"></div>

# 51. TeamViewer

Start teamviewer service: `systemctl start teamviewerd.service`

<div style="page-break-after: always; break-after: page;"></div>

# 52. Flatpak

```bash
pacman -S flatpak
flatpak install flathub com.usebottles.bottles
flatpak run com.usebottles.bottles

sudo ln -s /var/lib/flatpak/exports/bin/chat.rocket.RocketChat /usr/bin/rocket-chat
cp /var/lib/flatpak/app/media.emby.EmbyTheater/current/active/files/share/applications/media.emby.EmbyTheater.desktop  /usr/share/applications/
```

## 52.1. Firefox

```bash
flatpak install flathub org.mozilla.firefox
flatpak list to list apps
flatpak update <Application-ID> #(app-ID found in previous step)
# Added systemd service to update automatically flatpak apps (from arch wiki flatpak)
systemd-analyze --system unit-paths
```

<div style="page-break-after: always; break-after: page;"></div>

# 53. VM

## 53.1. Fix Resolution

- go to /etc/default/grub
- GRUB_GFXMODE=1024x768x32
- GRUB_GFXPAYLOAD_LINUX=keep
- grub-mkconfig -o /boot/grub/grub.cfg

## 53.2. SDcard on VM

- check with `fdisk -l` where is the sdcard (/dev/mmcblk0)
- unmount if mounted
- `VBoxManage internalcommands createrawvmdk -filename /path/to/file.vmdk -rawdisk /dev/mmcblk0`
- Go to the storage settings of the VM, add hard disk and select the .vmdk file created above
- `sudo usermod -a -G vboxusers goncalo`
- `sudo usermod -a -G disk goncalo`

<div style="page-break-after: always; break-after: page;"></div>

# 54. Latex

```text
/usr/share/texmf-dist/tex/latex/local
which mktexlsr
sudo path/to/mktexlsr or sudo $(which mktexlsr)---> update latex
```

<div style="page-break-after: always; break-after: page;"></div>

# 55. Plex

```text
docker stop plex
sqlite3 "config_docker/plex/Library/Application Support/Plex Media Server/Plug-in Support/Databases/com.plexapp.plugins.library.db"
PRAGMA default_cache_size = 20000; (com o ponto e virgula)
ctrl-D
docker start plex
```

<div style="page-break-after: always; break-after: page;"></div>

# 56. Format phone

## 56.1. Formatting

- `pacman -S android-tools`
- `adb shell - cd /data/adb/modules/quick* - find . -name "*.apk"`
- backup -> boot, system image, data
- `adb pull /sdcard/Fox` -> copy of the backup to pc
- `adb push zipname.zip /sdcard`  (no need to wipe to do this)
- `adb reboot bootloader`
- important partitions to wipe -> system, cache, data
- to flash recovery: `sudo fastboot flash recovery ficheiro-do-recovery.img`
- `pacman -S android-udev` (fastboot has no permissions)
- `treble check`
- `fastboot getvar all | grep “slot”`
- If there's any problem, I can always flash xiaomi rom (bookmarks)
- with command: `bash flash_all.sh` (only need to connect phone in fastboot mode)
- flash gapps after flahsing rom
- update firmware before new rom! Flashing the same way as the others
- Maybe need to really format data partition
- To update recovery, I can do it inside recover, flashing the zip
- To install, for example, Orange Fox, from TWRP, I can simply flash it from TWRP
- Installing lavender with gapps did not work... Need MindTheGapps

## 56.2. Connecting to PC

- Primeiro instalar termux
  - install fdroid and install termux from  there
- `pkg upgrade`
- `pkg install openssh`
- `touch ~/.ssh/authorized_keys`
- `chmod 600 ~/.ssh/authorized_keys`
- `chmod 700 ~/.ssh`
- copy key from pc to phone
- `cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys`
- `chmod 600 ~/.ssh/authorized_keys`
- run ssh: sshd
- kill ssh: pkill sshd
- `apt update && apt upgrade`
- port: 8022
- termux-setup-storage: (creates folder ~/storage)
  -shared: phone internal memory directory
  -external: sdcard (on sdcard: android-data-com.termux: Symlink external-1 points to a private Termux directory on external sdcard, i.e. /storage/XXXX-XXXX/Android/data/com.termux/files)
- pkg install tsu - using magisk this will give termux super user sudo
- After installing tsu, I can sudo chown /storage/XXXX-XXXX to be able to write on sdcard directly
- install jupyter-notebook:
  - `apt install clang python fftw libzmq freetype libpng pkg-config libcrypt`
  - `LDFLAGS="-lm -lcompiler_rt" pip install jupyter`
  - `pip install numpy` (ou pkg)
  - `pip install matplotlib`
  - run: `jupyter notebook`

- install termux-sudo-master : file in phone format folder (after installing tsu, dont
need this):

  ```bash
  pkg install ncurses-utils
  change to extraction directory of termux-sudo-master
  cat sudo > /data/data/com.termux/files/usr/bin/sudo
  chmod 700 /data/data/com.termux/files/usr/bin/sudo
  sudo su [-] -> gets me to root shell
  sudo <comand>
  ```

## 56.3. ARCH LINUX IN TERMUX

```bash
pkg update
pkg install curl bsdtar
curl -OL https://raw.githubusercontent.com/TermuxArch/TermuxArch/master/setupTermuxArch.bash
bash setupTermuxArch.bash
exit
pkg install vim
touch .bashrc
~/arch/startarch # at the bash prompt
pacman -Syyu sudo wget curl
sudo chown root:root /etc/resolv.conf
sudo chmod 644 /etc/resolv.conf
sudo passwd root
addauser <user>
exit
sudo passwd <user>
visudo
# And add your user's privileges under root's in the "User privilege specification" section: 
<user> ALL=(ALL) ALL
su - <user>
wget --no-check-certificate 'https://docs.google.com/uc?export=download&id=107Fh0l_p0ItVkUufOhP9to-OU_6KYhPW' -O fresharch.sh && chmod +x fresharch.sh && sudo bash fresharch.sh
add su - <user> to bash
# If you need to access shared storage, then cd into /storage/emulated/0
# create symlinks (ln -s) for storage
```

## 56.4. Process to format

- Boot to recovery
- Format system, data, cachr
- Reboot to recovery to reload partition table
- Install rom, format data, reboot to rom

## 56.5. Apps ADB

```bash
adb shell pm list packages
adb shell pm uninstall -k --user 0 NameOfPackage #(get name from app info, advanced)
adb uninstall com.example.myapp
adb shell content query --uri content://com.android.contacts/contacts
adb shell content delete --uri content://com.android.contacts/contacts/437413
adb shell content query --uri content://contacts/phones/  --projection display_name:number:notes
```

<div style="page-break-after: always; break-after: page;"></div>

# 57. Find Command

## 57.1. Error with mv command

By running the following command:

`find . -type f -name '*2019*' -exec mv {} ./backup_2019 \;`

I obtain the following errors:

```text
mv: ‘./backup_2019/2019-A.txt’ and ‘backup_2019/2019-A.txt’ are the same file
mv: ‘./backup_2019/2019-B.txt’ and ‘backup_2019/2019-B.txt’ are the same file
mv: ‘./backup_2019/2019-C.txt’ and ‘backup_2019/2019-C.txt’ are the same file
```

This happens because I am not ignoring the target directory to where I am moving the file.

The command:

`find . -path './backup_2019' -prune -o -type f -name '*2019*' -exec mv {} ./backup_2019 \;`

More ways of pruning:

`find . -maxdepth 1 \( -path "./Linux" \) -prune -o -type d -print`

`find . -mindepth 1 -maxdepth 1 \( -path "Some/Path" -o -path "./Linux" \) -prune -o -type d -print`

solves this issue.

Using the option `-maxdepth 1` should also solve the issue.


<div style="page-break-after: always; break-after: page;"></div>

# 58. Conky Desktop

`/usr/share/conky conky_maia` is the file I want. I have it saved in Linux backup.

## 58.1. Install conky-manager

Change in config:

```text
own_window yes
own_window_class Conky
own_window_type override
background yes
```

- To use the conky-manager, comment on config the line with: `exec --no-startup-id start_conky_maia`
- check for driver: lspci -k
- ifconfig: install net-tools : this allows to see the name of the device in use (eg. wlan0)
- add the files in conky-startup.sh like: `conky -c /path/to/file`
- add conky-startup to config

<div style="page-break-after: always; break-after: page;"></div>

# 59. EndeavourOS Stuff

- Might need to connect to network:

  ```bash
  nmcli d -> to determine the name of the wifi interface
  nmcli r wifi on
  nmcli d wifi list
  nmcli d wifi connect my_wifi password <password>
  ```

- Check wlan interface: `iw dev`
- Script photo nationalgeographic: `pacman -S python-pillow`
- Put touchpad file in `/etc/X11/xorg.conf.d` with:

  ```bash
  NaturalScrolling off
  AccelProfile -1
  ```

- Nao consigo obter em lyx o output por causa de ficheiros eps: `pacman -S ghostscript`
- Ao instalar o Mathematica, o script não gostou que o path tivesse um espaco

## 59.1. Relativamente ao barrier

- O nome dos dois pcs nao pode ser o mesmo;
- No ficheiro `/etc/systemd/system/barrier.service` tenho de ter:

  ```text
  [Unit]
  Description=Barrier Client mouse/keyboard share
  Requires=display-manager.service
  After=display-manager.service
  StartLimitIntervalSec=0

  [Service]
  Type=forking
  ExecStart=/usr/bin/barrierc --no-restart --name raspberrypi --enable-crypto 192.168.0.109
  Restart=always
  RestartSec=10
  User=pi

  [Install]		
  WantedBy=multi-user.target
  ```

  O important é em `--name` ter o nome do pc que eu pus no servidor (exemplo: no servidor, disse que o monitor se chamava goncalo-desktop... Entao, este é o nome que tenho de usar)

Note: Adicionar à config do i3 workspace_auto_back_and_forth yes

<div style="page-break-after: always; break-after: page;"></div>

# 60. Map Keyboard Keys

- Search for keycode:
  - `xmodmap -pk`
- Go to i3 config, add command: `exec_always --no-startup-id xmodmap -e "keycode 106 = backslash"`
- Note:
  - In the command above, keycode 106 is the key to be altered; backslash is the name of the the name of the key (In this example, it is backslash) and the keycode of the key I want to replace (which also has a name associated with it, in this case it was `KP_Divide`)

- Example:
  - `xmodmap -e "keycode 38 = a A aacute Aacute ae AE ae"`
  - Then:
  1. a: normal a
  2. A: shift + a
  3. á: altgr + a
  4. Á: shift + altgr + a

Using the example above, I can do: `exec_always --no-startup-id xmodmap -e "keycode 106 = backslash bar"`

This will include the | in the key when doing shift+key

On my keyboard, ç -> alt + ,

<div style="page-break-after: always; break-after: page;"></div>

# 61. Format Pen

## 61.1. Apagar partições

```bash
sudo fdisk -l -> para ver qual é a pen
sudo gdisk /dev/sdX -> em que X é o que encontro em cima
  o, enter
  n, enter, enter, enter
  0700
  w
```

## 61.2. Criar Partição

```bash
sudo mkfs.vfat /dev/sdX1
sudo mkfs.exfat # (for SD CARD)
```

## 61.3. Format pen with ISO

```text
sudo fdisk --list
dd if=manjaro.iso of=/dev/sd# status=progress
sync
```

If I want to install windows, use woeusb: `sudo woeusb --target-filesystem NTFS --device Win10_20H2_v2_French_x64.iso /dev/sdb`

<div style="page-break-after: always; break-after: page;"></div>

# 62. Borg Backup

## 62.1. Setup Steps

1) Create backup user in pi (do not add user no any groups):

  ```bash
  sudo useradd -m <username>
  passwd <username>
  ssh-keygent -t ed25519
  touch ~/.ssh/authorized_keys
  chmod 600 ~/.ssh/authorized_keys
  ```

2) Prepare repo directory:

  ```bash
  btrfs subvolume create /home/goncalo/HDD/@backups (btrfs subvolume create /path/to/mount/point)
  Add entry to fstab to mount this subvolume
  mkdir /mnt/backups/repo/name
  sudo chown <backup-user>:<backup-user> /mnt/backups/repo/name
  sudo chmod 770 /mnt/backups/repo/name
  ```

3) Init borg backup

  `borg init --encryption=keyfile ssh://backup-user@pi/mnt/backups/repo/name`

4) Borg mount (needs `pacman -S python-llfuse`)

  `borg mount path/to/repo::backup/name /mount/point`

## 62.2. MOUNT BACKUP AUTOMATICALLY

- Do it with systemd mount: needs a mount and .automount unit; This allows to export environment variables in the mount process;

- I'm mounting the backup repo using fstab (I mount it directly because I need the backup user) and then I use that to mount the borg backup through systemd mount; Eventually, this could be avoided if I used umask in borg (in umask the permissions subtract - 0077 results in 700; I probably want 0007)

- The systemd units to mount need to have the path where it is going to be mounted in the name. Example:
. Path where to mount: /mnt/borg_backup/backup_files -> Systemd unit name: mnt-borg_backup-backup_files.{mount,automount}

- The entry in fstab doesn't use the env variables specified in the systemd mount unit

<div style="page-break-after: always; break-after: page;"></div>

# 63. HDD Format

`sudo fdisk -l`

## 63.1. Delete Partitions

`sudo gdisk /dev/sdX` (where X is found from the previous step) and then select `d` and `w`

## 63.2. Create New GPT partition table

```text
sudo gdisk /dev/sdX
  - n
  - enter
  - enter
  - enter
  - w
```

## 63.3. Format Disk

`sudo mkfs.btrs -f /dev/sdX1`

## 63.4. Find UUID and check type

`sudo blkid`

## 63.5. Fstab

```text
UUID=d1e18a1a-1c64-458e-9aa3-e59cd9b8bd51       /home/goncalo/HDD2            btrfs   defaults,nofail,noatime   0       0
```

<div style="page-break-after: always; break-after: page;"></div>

# 64. Ubuntu

## 64.1. Fix ethernet unavailable

```text
[ifupdown]
managed=true
```

<div style="page-break-after: always; break-after: page;"></div>

# 65. PROBLEM: Unknown fs type vfat

Issue: Booted and got an error while mounting /efi during boot: /efi, unknown file system type vfat
What is happening: booting a different kernel from what is on /

Unpack unified kernel image to check kernel version:
- `objcopy -O binary --only-section=.linux linux.efi unpacked-vmlinuz`
- `file unpacked-vmlinuz`

Check current version: `ls /usr/lib/modules`

`sbctl list-bundles`

Generate new unified kernel image:

```text
sbctl bundle -s -i /boot/intel-ucode.img \
-l /usr/share/systemd/bootctl/splash-arch.bmp \
-k /boot/vmlinuz-linux \
-f /boot/initramfs-linux.img \
/efi/EFI/Linux/linux.efi
```

Edit `/etc/mkinitcpio.d/linux.preset`:

```text
ALL_config="/etc/mkinitcpio.conf"
ALL_kver="/boot/vmlinuz-linux"

PRESETS=('efi')

# BIOS
bios_image="/boot/initramfs-linux.img"

# EFI
efi_image="/boot/initramfs-linux.img"
#efi_options="--splash /usr/share/systemd/bootctl/splash-arch.bmp"
efi_microcode=(/boot/*-ucode.img)
efi_efi_image="/efi/EFI/Linux/linux.efi"
```

## 65.1. Some notes

- initramfs is the / before the actual / is mounted (it is mounted in ram) and provides basic utillities + systemd. It also includes some base kernel modules -> need to rebuild initramfs after kernel update
- systemd-bootx64.efi is just the bootloader
- efibootmgr writes on the motherboard directly
- linux.efi is an unified kernel image - contains kernel, initramfs, kernel arguments, ucode
- mkinitcpio gera o initramfs e depois produz o linux.efi
- vmlinuz-linux is the actual kernel

<div style="page-break-after: always; break-after: page;"></div>

# 66. Permissions

## 66.1. Fix permissions

- `sudo pacman-fix-permissions`
- check ssh to fix key permissions
- `stat -c "%a %n" /etc/ssh/*` -> outputs permissions in numbers

I have made a script with a file which has the correct permissions which I got from alex pc

<div style="page-break-after: always; break-after: page;"></div>

# 67. Raspberry Pi

- Needed to systemctl enable sshd inside chroot (chroot root/@)
- p10k configure to configure p10k theme for zsh
- For username in zsh prompt: uncomment context line in .p10k file in POWERLEVEL9K_LEFT_PROMPT_ELEMENTS
- In order for the systemctl --user to work, need to set UsePAM yes in /etc/ssh/sshd_config
- In rebelo script change:
  - rebelo-pi to goncalo-pi
  - change also the Disk to avoid potential problems

- file `/etc/iptables/iptables.rules`:

  ```text
    *filter
    :INPUT ACCEPT [0:0]
    :FORWARD ACCEPT [0:0]
    :OUTPUT ACCEPT [0:0]
    COMMIT
  ```

- before finishing formating I need to:
  - change iptables.rules
  - change sshd_config (port and pw authentication)
  - enable sshd service

- on sdcard, aarch64 did not work. Need to change config/config.sh:
  - ARCH_CPU_BRAND=armv7h
  - ARCH-KERNEL=linux-rpi

- In order to be able to build the packages to arm architecture from arch x86_64 need to install:
  - qemu-user-static-bin
  - Other dependencies:
    - arch-install-scripts
    - uboot-tools
    - aria2
    - iwd
    - gnu-netcat (for nc)
    - arp-scan
    - exfatprogs (for mkfs.exfat)

- Edit `/boot/config.txt` for overclock

  ```text
    enable_uart=1 (this screws up the OC)
    over_voltage=6
    arm_freq=2000
  ```

- In order for the ssh-agent to work, add to /etc/ssh/sshd_config:
  - UsePAM yes

Don't forget systemctl --user cannot be ran with sudo

For docker to work, don't forget to change the UID in everyfile.
The error:

`Failed to load config file "/run/secrets/rclone_conf": open /run/secrets/rclone_conf: permission denied`

was because I did not change the UID in the image for rclone Docker

Final step: `docker-compose build`

- stress test: stress -c 4 -t 900s

- https://healthchecks.io/

- To update firmware: pacman -S rpi-eeprom:
  - rpi-eeprom-update (checks version)
  - rpi-eeprom-update -a (updates)

<div style="page-break-after: always; break-after: page;"></div>

# 68. Plasma

## 68.1. Packages

```text
plasma-desktop
plasma-wayland-session
plasma-workspace-wallpapers
plasma-systemmonitor
plasma-nm
plasma-pa
plasma-browser-integration
powerdevil
bluedevil
kdialog  # for native dialogs in some apps
breeze breeze-gtk
kwrited
phonon-qt5-gstreamer
kde-gtk-config
xdg-desktop-portal xdg-desktop-portal-kde xdg-desktop-portal-gtk
khotkeys
```

## 68.2. Launch

```bash
# Wayland
export MOZ_ENABLE_WAYLAND=1
export XDG_SESSION_TYPE=wayland
exec startplasma-wayland

# X11 
exec sx startplasma-x11
```

## 68.3. Autostart

Check the following paths

```text
~/.kde/Autostart
~/.kde/share/autostart
~/.config/autostart
~/.local/share/autostart
/etc/xdg/autostart
/usr/share/autostart
```

## 68.4. XDG Autostart directories

Place Desktop entries (i.e. .desktop files) in the appropriate **XDG Autostart directory**:

- user-specific: `$XDG_CONFIG_HOME/autostart` (~/.config/autostart by default)
- system-wide: `$XDG_CONFIG_DIRS/autostart` (/etc/xdg/autostart by default)

To disable a system-wide entry, create an overriding entry containing `Hidden=true`.

## 68.5. Autostart Manager

The program scans `$HOME/.config/autostart/` for applications and login scripts, `$HOME/.config/plasma-workspace/env` for pre-startup scripts and `$HOME/.config/plasma-workspace/shutdown` for logout scripts to check what programs and scripts are already there and displays them. However, applications in `/etc/xdg/autostart` are also launched.

To autostart an application, navigate to System Settings > Startup and Shutdown > Autostart and add the program or shell script of your choice. For applications, a .desktop file will be created, for login scripts, a .desktop file launching the script will be created.

If a desktop file under `$HOME/.config/autostart/` has `OnlyShowIn=XFCE;`, then it will not be autostarted.

## 68.6. Disable kdeconnect

First we need to avoid kdedconnect to autostart:

`cp /etc/xdg/autostart/org.kde.kdeconnect.daemon.desktop ~/.config/autostart/`

Now edit the file `~/.config/autostart/org.kde.kdeconnect.daemon.desktop` and add `Hidden=true`. Actually you can even remove everything else, because only the file name has to be identically so it's "overriden". So it looks like:

```text
[Desktop Entry]
Hidden=true
```

Now the autostart service is disabled, but this isn't enough. We also need to "disable" the d-bus service:

```bash
mkdir -p ~/.local/share/dbus-1/services/
cp /usr/share/dbus-1/services/org.kde.kdeconnect.service ~/.local/share/dbus-1/services/
```

Edit the file `~/.local/share/dbus-1/services/org.kde.kdeconnect.service`  and change Exec to `/usr/bin/false` so the file looks like:

```text
[D-BUS Service]
Name=org.kde.kdeconnect
Exec=/usr/bin/false
```

`/usr/bin/false` will return with a "error" return code (because it returns with 1 and not 0), so your logs (via journalctl) may display the process couldn't start or failed. But that shouldn't matter.

Now kdeconnectd should not run anymore after you logout and login again.

## 68.7. Shortcuts

- "Switch to Next Screen" shortcut to work: you need to check "Separate screen focus" option first from System settings → Window behavior → Window Behavior (on the left side) → Separate screen focus
- Logout Menu: Shortcuts → Session Management → Logout (default: ctrl+alt_del)
- Screen Lock: Workspace Behavior → Sreen Locking (also, disable automatic screen lock here)
- "Switch to Screen 0": Meta+Ctrl+Right
- "Switch to Screen 1": Meta+Ctrl+Left
- "Switch to Window to the Left": Meta+Alt+Left
- "Switch to Window to the Right": Meta+Alt+Right

## 68.8. Fixing hanging service on shutdown

First atempt: `sudo rm /usr/share/dbus-1/accessibility-services/org.a11y.*`

Add:

`NoExtract = usr/share/dbus-1/accessibility-services/org.a11y.*`

to makepkg.conf.

## 68.9. Config

### 68.9.1. Startup and Shutdown → Background Services

- Remove Search Folder Updater (also go to Search → File Search and untick `Enable File Search`)

### 68.9.2. Startup and Shutdown → Desktop Session

- [x] Start with an empty session
- [x] Confirm Logout
- [x] Offer Shutdown Options
- [x] End Current Session

### 68.9.3. Power Management → Energy Saving

- Untick Screen Energy Saving

### 68.9.4. Display and Monitor → Night Color

- Activate

### 68.9.5. Window Management → Task Switcher

- Filter Windows by: Virtual desktops and Screens (**current** in both)

### 68.9.6. FlameShot

I should not use the shortcut option for flameshot that comes by default. Instead do:

- Go to Settings > Shortcuts > Custom Shortcuts
- Right click > New > Global Shortcut > Command/Url
- Select trigger and Command/Url to `/usr/bin/flameshot gui`

### 68.9.7. Task Bar

- Add "Task Manager" widget to each panel
- Right-click on an item in Task Manager -> Configure Task Manager
- Behavior tab -> Filter: Show only tasks from the current screen
  
<div style="page-break-after: always; break-after: page;"></div>

# 69. Regex

```bash
# Lessons: need -n flag which disables automatic printing
# Need to escape the plus sign
sed -n 's/.*\(FOR-ICU-[0-9]\+\).*/\1/p' List_Of_Reqs.txt 
```

<div style="page-break-after: always; break-after: page;"></div>

# 70. Compare files

```bash
# This command will output lines unique to file_2. So, if output is empty, then all file_2 lines are contained in the file_1.
comm -13 <(sort -u file_1) <(sort -u file_2)
```

<div style="page-break-after: always; break-after: page;"></div>

# 71. Fiddler

First, you should enable the Allow remote computers to connect setting in Fiddler

1. Open Fiddler and select Tools -> Options
2. Choose the Connections tab
3. Select the Allow remote computers to connect checkbox to enable the setting
4. Restart Fiddler in order the changes to take effect

Fiddler is now listening on port 8888 (this is the default port, you can change it from the setting above).

Once Fiddler is listening, we should use it as a proxy in Android.

1. Open the WiFi menu.
2. Tap and hold on your current network to show the network details
3. Choose the Manage network settings option
4. Check Show advanced options checkbox
5. Choose Manual from the Proxy dropdown list
6. Type your IP address in the Proxy host name field
7. NOTE: You can check your IP address by hovering over the Network Connection icon in the Fiddler toolbar.
8. Type the Fiddler listening port (8888 by default) in the Proxy port field
9. Click Save to apply changes

With the current setup you should be able to capture HTTP traffic. However, if you try to open any HTTPS website, you’ll get the This site’s security certificate is not trusted! error. To fix this, you should trust the Fiddler root certificate.

NOTE: By default, Fiddler-generated certificate is valid for 5 years. However, this can cause ERR_CERT_VALIDITY_TOO_LONG error in Chrome on Android. To fix this:

1. Run about:config in Fiddler QuickExec.
2. Create new variable fiddler.certmaker.ValidDays with value 820

Then, you can proceed with installing the Fiddler Root certificate as follow:

1. In your browser, navigate to http://ipv4.fiddler:8888
2. Download the Fiddler root certificate.
3. Install the certificate on your device.

Now you should be able to capture HTTPS traffic too.

<div style="page-break-after: always; break-after: page;"></div>

# 72. Termux

Termux should be installed from F-Droid, both in TV and phone.

Besides termux, install (also using F-Droid) Termux:API, Termux:Boot, Termux:Widgets.

In terms of permissions, both in TV and Phone, allow termux to `Display Over Other Apps`.
In TV, in order to get this setting, go to settings -> Apps -> Termux and it should be there.

Note: In TV, in order to have wireless debug, need to allow USB debugging in developer options and then allow the connection with the pc.

## 72.1. Termux Brightness

This needs termux:api. Termux:Api should be allowed to `Modify system settings`.

With termux:widgets, all scripts placed under `~/.shortcuts` will be able to be selected as a shortcut with termux:Widget. 

Then, in order to control brightness use `termux-brightness`. Example:

```bash
if [[ "$(uname -o)" == "Android" ]]; then
  termux-brightness 255
  trap "termux-brightness 40; exit" SIGINT
fi
```

## 72.2. TV url opener

Use Termux:Boot in order to start sshd server.

Create script under `~/bin/` name `termux-url-opener`:

```bash
#!/data/data/com.termux/files/usr/bin/sh

ssh 192.168.200.70 -p 8022 termux-open-url "$1"
```

<div style="page-break-after: always; break-after: page;"></div>

# 73. VPN Critical

Some commands: 

```bash
nslookup
 > server <Server_IP>
 > name.company.com

resolvectl query name.company.com

nmcli device show wlp1s0 | grep DNS
```

On Ubuntu: `/etc/NetworkManager/NetworkManager.conf` append the following lines:

```text
[keyfile]
unmanaged-devices=interface-name:vpn*,except:interface-name:enp0s3;interface-name:wlan*
```

<div style="page-break-after: always; break-after: page;"></div>

# 74. Secure Boot

## 74.1. Steps for secure boot

1) Setup motherboard in setup mode. In order to do that, go to `Secure boot options` and `Delete all Signatures`;
2) Install booster: `pacman -S booster`
3) Check `sbctl status` and see if `Setup Mode` is `Enabled`
4) After, create keys

  ```bash
  sbctl create-keys
  chmod 600 /usr/share/secureboot/keys/**/*.key
  ```

5) If `Setup Mode` is Enabled, then enroll keys:

   ```bash
   sbctl enroll-keys --microsoft
   ```

6) Keep the keys in the efi partition for easy re-enrollment: `mkdir -p /efi/keys; cp /usr/share/secureboot/keys/**/*.pem /efi/keys`
7) `mkdir -p /efi/EFI/Linux`
8) Finally,

```bash
# Bundle and sign kernel
sbctl bundle -s \
    -i "/boot/$ARCH_CPU_BRAND-ucode.img" \
    -k "/boot/vmlinuz-$ARCH_KERNEL" \
    -f "/boot/booster-$ARCH_KERNEL.img" \
    "/efi/EFI/Linux/booster-$ARCH_KERNEL.efi"

# Sign systemd-boot
sbctl sign -s "/efi/EFI/systemd/systemd-bootx64.efi"

# Re-generate all
sbctl sign-all -g
```

9) Don't forget to have the same keys in the main system and in the recovery system
10) After doing this, remove `mkinitcpio`- I should only remove it after, otherwise something might go wrong
11) On recovery, if it wasn't setup like this, copy first the keys to the recovery partition; install booster (note that I need `arch-chroot` - it mounts necessary stuff for the chroot comparing to `chroot`) and run the `sbctl bundle` command (where the efi needs to be renamed, careful!!!!!) and then `sbctl sign-all -g` (although I think this last sign is not necessary). Note that do not need to sign the bootloader again.

Note: If I already had windows installed, this would work out of the box because of the `--microfost` flag.

<div style="page-break-after: always; break-after: page;"></div>

# 75. Helix

The helix mindset is that we always highlight something before performing an action.

To install md preview, run `cargo install --git https://github.com/euclio/mdpls` and then add to `languages.toml`:

```text
[[language]]
name = "markdown"
language-server = { command = "/path/to/mdpls" }
config = { markdown.preview.auto = true, markdown.preview.browser = "firefox" }
```

## 75.1. Some commands

1) Modes: insert, visual, normal, space, go-to, match
2) File picker: space mode -> f
3) While in file picker, to open in a vertical split: Highlight target file and press Ctrl + V
4) Alt + . do redo a command
5) In order to remove a highlight, press ";"
6) Press "C" to delete a highlighted section and start writing
7) "s" (select) is basically a search within the selected text. If we do this and then press "c", we can do a find a replace
8) Use "," to get rid of multiple cursors
9) Use "x" to highlight an entire line, in normal mode. Subsequent presses of "x" will highlight subsequent lines
10) "]+f" will highlight an entire function
11) "[+c" will go to the previous class/struct
12) "]+a" to cycle through all function parameters
13) In space mode, press "s" to open a symbol picker and "S" for the entire workspace  
14) "Space + r" to rename a symbol
15) "Space + a" to get code actions
16) "g+d" to go to definition. Here, it helps to do "Crtl + i" and "Ctrl + o" to go back to where we came from
17) "g+r" will show all places where something is referenced
18) "Shift+r" will replace the current highlight with what we yanked before
19) Pressing `"` allows to select the register to which we want to yank something. Then, press the letter to save to and yank

<div style="page-break-after: always; break-after: page;"></div>

# 76. Pihole

## 76.1. Configuration

By default, it won't work since, by using systemd-resolved stub listener, port 53 will be occupied. For that, the stub resolver should be disabled with:

`sudo sed -r -i.orig 's/#?DNSStubListener=yes/DNSStubListener=no/g' /etc/systemd/resolved.conf`

This will not change the nameserver settings, which point to the stub resolver thus preventing DNS resolution. Change the `/etc/resolv.conf` symlink to point to `/run/systemd/resolve/resolv.conf`, which is automatically updated to follow the system's netplan: `sudo sh -c 'rm /etc/resolv.conf && ln -s /run/systemd/resolve/resolv.conf /etc/resolv.conf'`. After making these changes, you should restart systemd-resolved using `systemctl restart systemd-resolved`.

Since raspberry uses dhcpcp, it will overwrite the `/etc/resolv.conf`. In order to avoid this we can disable the hook `/usr/lib/dhcpcd/dhcpcd-hooks/20-resolv.conf`. Do so by adding the following to the last section of `/etc/dhcpcd.conf`:

```text
nohook resolv.conf
```

The above configuration does not seem to work well with tailscale, since systemd-resolved will still use `/run/systemd/resolve/resolv.conf` and tailscale renames `/etc/resolv.conf` to `/etc/resolv.conf.bak` and this keeps pointing at `/run/systemd/resolve/resolv.conf`, and writes a new `/etc/resolv.conf` that does not seem to be used by systemd-resolved - then, the tailscale dns configuration is not in use.

In this case, simply disable systemd-resolved and use the tailscale `/etc/resolv.conf` directly:

```text
# resolv.conf(5) file generated by tailscale
# DO NOT EDIT THIS FILE BY HAND -- CHANGES WILL BE OVERWRITTEN

nameserver 100.100.100.100
search taildbd36.ts.net
```

<div style="page-break-after: always; break-after: page;"></div>

# 77. Thunderbird

## 77.1. Critical Account

### 77.1.1. Configure

Incoming:

- IMAP
- Server hostname: outlook.office365.com
- Port: 993
- SSL: SSL/TLS
- Authentication: Oauth2

Outgoing:

- Server hostname: smtp.office365.com
- Port: 587
- SSL: STARTTLS
- Authentication: Oauth2

Username (Incoming and Outgoing): email

### 77.1.2. Calendar

- Install TBSync extension
- Install Provider for Exchange ActiveSync
- In TBSync, add account (exchange) and sync calendar

<div style="page-break-after: always; break-after: page;"></div>

# 78. XDG-DESKTOP-PORTAL

Fix applications taking long to on startup:

- Install xdg-desktop-portal-gtk: `pacman -S xdg-desktop-portal-gtk`
- Uninstall xdg-desktop-portal-wlr: `pacman -R xdg-desktop-portal-wlr`
- Add i3 to `UsrIn=gnome;i3` in `/usr/share/xdg-desktop-portal/portals/gtk.portal`

Also add to .zprofile the following exports:

```bash
export XDG_SESSION_TYPE=x11
export XDG_CURRENT_DESKTOP=i3
export GDK_BACKEND=x11
```

<div style="page-break-after: always; break-after: page;"></div>

# 79. Parsec

## 79.1. Wake on lan

For wake on lan to work, check: `ethtool interface | grep Wake-on`. The output should be `g` and it is required for `WoL` to work. It can be set with `ethtool -s interface wol g`. If using `NetworkManager`, this can be made persistent by going into the ethernet configuration inside network manager and enabling the magic packet.

## 79.2. Wake PC

- ssh to rpi and run: `wol -v bc:5f:f4:83:32:cc`.
- In desktop, `systemctl reboot --boot-loader-entry=auto-windows`

<div style="page-break-after: always; break-after: page;"></div>

# 80. Misc

1) By disabling all F86 binds in config and installing xfce-power-management (which needs to be started in config and need to get config from Manjaro/Home/.config) and installed pa-applet-git, pavucontrol and pulseaudio (initiated in config) all the F86 binds work.
2) It is preferable to have xfce4-notify (initiated in config by running `/usr/lib/xfce4/notifyd/xfce4-notifyd`) than dunst... Better notifications. Check i3 config and uninstall dunst (in endeavour).
In manjaro, do: `sudo mv /usr/share/dbus-1/services/org.knopwob.dunst.service{,.disabled}`
3) Bluetooth:
   - pacman -S pulseaudio-bluetooth
   - pulseaudio -k
   - yay -S bluez-hciconfig
   - hciconfig -> lists bluetooth interfaces
   - sudo hciconfig hci1 down -> turn off specific interface
4) Sticky xrandr:
   - `xrandr --output eDP --primary`
   - `pacman -S autorandr`
   - `autorandr --save laptop`
5) FSTAB

    ```
    sshfs : jose@pi:/ /mnt/rebelo-pi fuse.sshfs noauto,x-systemd.automount,_netdev,user,idmap=user,follow_symlinks,identityfile=/root/.ssh/id_rsa,allow_other,default_permissions,uid=1995,gid=1995,noatime,reconnect,ServerAliveInterval=45,ServerAliveCountMax=2 0 0
    ```
6) SYMBOLIC LINKS
   - `ln -s /complete/path/to/original/file /complete/path/to/target/file` (the target file will be a "pointer" to the original file, but it's like the file is in the new target location)
   - `ln -sr /relative/path/to/original/directory /complete/path/to/target/directory` (the target directory will be a link to the first; the -r flag means relative)
   - The `-f` flag will force the link, meaning it delets the target file/directory if it exists
   - Remember to always use complete paths and not relative paths if the -r flag is not specified
7) SSH
   - I can run commands over ssh like this: `ssh user@host 'command'`
     - Example: `liplisboacluster 'echo $(hostname)'` -> prints hostname
   - Writting on a remote file:

    ```bash
    echo 'Some Text' | ssh user@remotehost -T "cat > /remotefile.txt"
    # (-T flag fowards stdin local through ssh)
    cat ~/.ssh/id_rsa.pub | ssh user@remote.host 'dd of=.ssh/authorized_keys oflag=append conv=notrunc'
    ```

   - In order to have several ssh keys, do:

    ```bash
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    eval $(ssh-agent)
    ssh-add ~/.ssh/id_rsa2 (newly created key)
    ```

   - In order to have ssh-agent always running, check ~/.config/systemd and .zshrc
   - `systemctl --user enable ssh-agent.service` (probably don't need to do this since I have a backup of .config/systemd)
   - Check services: `systemctl --user list-unit-files | grep enabled`
   - Check services (all): `systemctl list-unit-files | grep enabled`
   - Also, need to add to zshrc a function to load keys, since ssh-add only works for the current session
   - To have a proxy:
  
    ```
    Host 10.0.10.3
    User goncalo
    ProxyCommand ssh goncalo@jgroboredo.ddns.net -W %h:%p
    ```

   - If ssh service fails to start with error: Start request repeated too quickly, do the following:
  
    ```bash
    sudo systemctl stop sshd.socket and sshd.service
    sudo /usr/bin/sshd -d
    #If message from above command states a permission issue:
    sudo chmod 400 /etc/ssh/ssh*key
    ```
8) Firefox crash
   - Seems like it was the gtk theme from popOS that made firefox to crash
   - In sway, if font problems, export GTK_USE_PORTAL=1
   - In what concerns crashes, picom with xrender crashes! Need to use glx
   - Today, 10/08/2021, firefox started crashing. Disabled picom and it did not solve the problem. Updated picom config from arch linux wiki, did not help. Firefox->Settings->Performance did not change anything
   - Starting firefox from terminal does not seem to solve the problem. Does not output any errors.
   - Testing launching firefox and terminal from i3 bind with the flag --no-startup-id -> doesnt work
   - Testing google-chrome-stable; disabled guake
   - Google-chrome also crashed; However, it recovered after a few seconds, similar to what previously happened to vscode. It seems like a X11 problem. Moved to sway.
   - Testing again firefox crashes on i3. For now, uninstalled xf86-video-intel. Since then, no crashes yet.

   - FIREFOX SLOW START:
     - about:config
     - set 0 to all widget.use-xdg-desktop-portal
9) ARCH NOT BOOTING IN VM
   - On a recent installation of arch on a VM, it did not boot after installing the custom grub-theme. In order to solve this, either chroot or open a terminal using ctrl+alt+F2. There, delete the grub theme in /usr/share/grub/themes and after that run grub-mkconfig -o /boot/grub/grub.cfg
   - The above solution doesn't work. In fact I am very dumb. This was only related with the fact that I have a intel config file in /etc/X11/xorg.d.... DUMBBBB
10) FIND UUID OF DISK
    - sudo blkid | grep UUID=
11) FIX YAY
    - Error: yay: error while loading shared libraries: libalpm.so.11:  cannot open shared object file: No such file or directory
    - Fix: rebuild yay:

    ```
    cd /tmp && git clone 'https://aur.archlinux.org/yay.git' 
        && cd /tmp/yay && makepkg -si && cd ~ && rm -rf /tmp/yay/
    ```

12)  FIX PAMAC	
     - `Error: libpamac-aur: /etc/pamac.conf exists in filesystem`(owned by pamac-aur) 
     - Fix: `pacman -R pamac-aur && yay -S pamac-aur`
13) FIX TIME
    - `sudo ntpd -qg`
    - install ntp
    - `sudo ntpdate pool.ntp.org`
    - `timedatectl set-ntp true`
14) CHECK RAM
`sudo dmidecode -t memory`
15) lxrandr to change monitors
16) CONFIG LINUX ACCOUNT
    
    ```bash
    sudo useradd -m test
    userdel <nome de utilizador do utilizador>
    adduser username sudo
    /etc/ssh/sshd_config # Allow pubkey and add authorized_keys file;
    chsh -s $(which zsh)
    sudo service ssh restart
    # For redmine: couldn't add repos to redmine: change permissions: 
    chmod 775 /path/to/dir
    ```

17) Dmenu-extended
     - For apps to open I need desktop files to associate a given mimetype to a binary
     - After doing the above step, rebuild cache
18) NetworkManager/Network interface stopped working
    - Solution: boot to a pen with manjaro and reboot
    - See logs:

    ```bash
    find /sys/class/net -follow -maxdepth 2 -name wireless
    cat /proc/net/wireless
    iw dev
    sudo iw dev wlp0s20f3 connect "ROBOREDO"
    sudo dmesg | grep firmware
    sudo dmesg --level=emerg,alert,crit,err
    lspci | grep net
    lsmod
    sudo ls /etc/netctl/interfaces
    ```

19) Rebuild all yay packages depending on python:
  `yay -S $(pacman -Qoq /usr/lib/python3.9) --answerclean All`
20) nc : install `pacman -S gnu-netcat`
21)  Can add stuff to path in .xinitrc; a user systemd service needs to have WantedBy=default.target and not multi-user
The rclone command will not work in a user service since systemd doesn't have access to env variables. For that, just add a env.conf file to .config/environment.d/ (check printenv)  
22) Delay a systemd service:
    ```bash
    [Service]
    ExecStartPre=/bin/sleep 30 
    ```

23) DMZ - portas abertas para toda a internet
24) `dhcpcd -T eth0` - check dns
25) PERMISSIONS
    ```bash
    chown -R root:root /etc
    find /etc -type f -exec chmod 644 {} +
    find /etc -type d -exec chmod 755 {} +
    chmod 755 /etc/init.d/* /etc/rc.local /etc/network/* /etc/cron.*/*
    chmod 400 /etc/ssh/ssh*key
    check desktop_dotfiles
    ```
26) Need imagemagick for blurlock
27) samba

    ```bash
    smbclient '//print-server.critical.pt/Drivers/' -U critical/jgroboredo (smbclient '//ip/Directory')
    smbclient '\\files.critical.pt/Repository' -U critical/jgroboredo
    get file
    ```

28) bluedevil; bluedevil-wizard; systemctl start bluetooth;
    pavucontrol: High Fidelity Playback (A2DP Sink, codec LDAC)
    blueberry-tray
29) `sudo lsof -i -P -n | grep LISTEN`
30) bash gum package
31) gtk-update-icon-cache -f -t .icons ou (/usr/share/icons/)
 		 Add icon field in desktop file - only the name.png
