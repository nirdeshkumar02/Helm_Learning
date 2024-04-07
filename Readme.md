## HELM

Helm is an open-source third-party utility, now known as the package manager for Kubernetes, focused on automating the Kubernetes applications lifecycle in a simple and consistent way.
The objective of Helm as package manager is to make an easy and automated management (install, update, or uninstall) of packages for Kubernetes applications, and deploy them with just a few commands.

## Benefits of using Helm

1. **Manage Complexity:** Charts describe even the most complex apps, provide repeatable application installation, and serve as a single point of authority.

2. **Easy Updates:** Take the pain out of updates with in-place upgrades and custom hooks.

3. **Simple Sharing:** Charts are easy to version, share, and host on public or private servers.

4. **Rollbacks:** Use helm rollback to roll back to an older version of a release with ease.

## For More; [Follow HELM Documentation](https://helm.sh/)

## What We Cover in practice_1 and practice_2
1. Helm Components
2. Customizing Chart Parameter
3. Working with Helm
    1. Basic - Parameterizing and Refrencing values from values.yaml
    2. Functions - work on the refrence value like uppper, indent, title, range etc.
    3. Pipeline - pass refrence value to another function like `{{ .Values.name | upper }}`
    4. Conditionals - How we can use if/else like `{{ if .Values.serviceAccount.create }}` then create service accound else no. 
    5. Short the Refrence using With Blocks
    6. Named templates - having common things under `__helpers.tpl` and then include them in objects.
    7. Chart Hooks - Action to perform after some helm action like what to do before/after helm install or helm upgrade.
