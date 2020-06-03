# awesome-patches
Usage

1. add `patch-package` to your project

```shell
npm i -S patch-package

or 

yarn add patch-package
```

2. download patch file and put it into folder `patches`

3. run `npm` or `yarn` to patch it

```
npx patch-package

or 

yarn patch-package
```

4. you can add postinstall to `package.json` to automating this process.

```
"scripts": {
    "postinstall": "patch-package"
}
```

