## revel-docker

a revel(a Go web framework) container better than others.

I searched google and expect to find a good enough revel container, but I fail.
So I build it.

## Usage

```bash
docker run -it -v /go/src:/go/src -p 9000:9000 annatarhe:revel revel run github.com/username/project
```

you have to set the volumn to your Go root `src/` not just the project dir!

