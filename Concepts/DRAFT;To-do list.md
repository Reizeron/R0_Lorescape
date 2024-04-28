What to do next:

- [x] Change website icon
	- done, only need to push changes
- [x] Create bat files for preview building and pushing changes:
	  - `npx quartz build --serve`
	  - `npx quartz sync`
	  - Don't remember if I need to echo off or something
	  - Need bat files for quick preview build using a different content folder:
	   `-d` or `--directory`: the content folder. This is normally just `content`
- [ ] Write scripts to transfer website content from the obsidian vault
	- Topics only?
	- Alternatively, create a symlink to the Obsidian vault
		- Enabled symlinks in git settings, will try again.
- [ ] Write scripts to bulk create links between topics
	- It can also remove broken links?
- [x] Replace the mountain emoji in title with the custom scroll icon
    - maybe change the color to MW text color too?
	- `D:\Repositories\quartz\quartz\components\PageTitle.tsx`
		Must add something like this:
		```<img src="/static/icon.png">```		```
- [ ] etc.