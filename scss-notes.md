#### 11/3/23
### Switching from @import to @use/@forward for Sass

- in each of 7 folders from 7-1 architecture, put a "_index.scss" partial file.
- in each partial file, @forward the other files from the folder (ex: '@forward "../base/reset"')
- outside of the 7 folders, inside the scss folder, put a main scss file (like previously)
- in the main scss file, @forward the scss folders (which automatically pulls in the index file for that file, which contains and forwards the partials)
- in main scss file, only need to forward the folders that contain files that contain style rules (ex: "body{...}) and not the variables, mixins, etc
- in other words, this means that the main scss file is only needed for components (and the like), not variables (and the like)
- variables, mixins, etc can be forwarded out of their folder (usually abstracts) via their index partial scss file, and then called in the file where they are needed with @use
- to call variable with @use: call the abstracts (or respective folder) with @use at the top of the file where it will be needed
- then when calling the specific variable name, don't forget the namespace
  - ex: '@use "../abstracts"' pulls in abstract folder forwarded index partial, which pulls in forwarded variables partial, which contains the variables
  - putting "@use..." as above at top of reset partial allows for use of variables from abstracts in reset partial
  - ex: "body{background-color: abstracts.$variable-name}"
  - in above ex, "abstracts" is the namespace
- also don't forget to consider relative paths of the index files between 7-1 folders (which is why "../" is in front of "abstracts" folder name in above example, because it's being called from inside a different 7-1 folder
- namespace can be reassigned when pulling into file, ex: "@use "../abstracts" as abs"
- within file, when pulling in with "@use" you can also set the namespace with "...as *" which eliminates the need to use the namespace in front of the called variables/mixins/etc below it in the file, but this is not usually recommended
- because the advantage to recording the namespace as part of the variable, etc is to track where it comes from and prevent conflicts (ex two different values assigned to the same variable name)


### One Interpretation of 7-1 Sass Architecture
- base: general/ global styles
- components: individual components
- abstracts: colors, fonts, (variables), etc
- layouts: page-related
- utilities: reusable classes
