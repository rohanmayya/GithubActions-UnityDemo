# GithubActions-UnityDemo
Quick tutorial on how to setup CI/CD with GitHub Actions for your Unity project

Here I'm going to outline a set of super simple steps to get started with GitHub Actions for your Unity build.

Head over to .github/workflows. You will see 2 .yml files there.
The first is `activation.yml`.
All actions use a Unity installation, which needs to be activated. `activation.yml` comes straight from game.ci's docs, you're free to modify it as you deem fit.

`main.yml` is where you can setup your own build workflow.
In my case, I'm caching my assets, uploading my build to artifacts, and (for now) creating a Windows64 build because that's all I care about.
