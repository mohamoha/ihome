# How to delelop this module

---

---


## 1. Install spm & apm

```bash
$ npm install apm -g
$ spm doctor
```

## 2. Clone the repo

```bash
$ git clone git@github.com:aliceui/ihome.git
```

## 3. Start watching the document site

```bash
$ cd ihome
$ spm doc watch
```

Then open http://127.0.0.1:8000, browser the demos.

## 4. Update version if need

## 5. Edit the source files in `src/`

Debug the demo at http://127.0.0.1:8000. Don't forget `git commit`.

## 6. Finish your development, publish this module

```bash
$ spm build
$ spm publish
$ spm doc publish
```

## 6. Push to Github

```bash
$ git tag x.x.x
$ git push origin master
$ git push origin x.x.x
```
