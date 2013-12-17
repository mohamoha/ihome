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

## 6. Build and deploy your files to development envirnment.

```bash
$ spm build
$ spm deploy
```

## 7. Push to Github

```bash
$ git tag x.x.x
$ git push origin master
$ git push origin x.x.x
```

## 8. Publish this module

when your project is ready being published.

```bash
$ spm doc publish
$ spm publish
```

## 9. Up to alipay cdn.

> https://a.alipayobjects.com/alice/ihome/x.x.x/index.css
