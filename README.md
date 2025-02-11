# Dashfy ( -,-) 
Replace spaces and underlines by dashes

### Setup
1. Clone this repository
```
git clone https://github.com/henriquehorbovyi/dashfy
```
2. Give permission to execute to all scripts


3. Export dashfy directory to your $HOME path

```kotlin
// Chose where to place your dashfy directory and change the path accordingly
export PATH="$HOME/dashfy"
```
4. Use it with Git (Optional)

You can create an alias to the `git-switch-extension` which executes a `git switch -c $(dashfy $@)`, meaning that whatever text you pass as a branch name it's going to be dashfied.

```kotlin
// This is the alias name I use
alias gsw='git-switch-extension'
```
Obs: As this step is optional, you can obviously delete `git-switch-extension` file if you won't use it

### How to use

```kotlin
dashfy hello world
// output: hello-world 
```

```kotlin
dashfy Hello World
// output: hello-world
```

```kotlin
// on a git repository run
git switch -c $(dashfy My lovely ticket name)

// result: Creates a branch called my-lovely-ticket-name and switch to it
// or you can run the alias
gsw My lovely ticket name
// Result: Creates and switch to a branch called my-lovely-ticket-name
```

