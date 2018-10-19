# Git Mirror

_Easily make a mirror for your git repo._

Make separate directory for your mirror jobs, because it's important and it should be part of your backup schedule.
Clone or download bash script from here `https://github.com/borvelt/repository-mirror.git`

```bash
git clone https://github.com/borvelt/repository-mirror.git git-mirror
cd git-mirror
```

## Prepare

Open gitMirror bash file and find two words `REPOS` and `MIRROR_REPOS` and remove values and enter your own repositories.

**notice**: there's a point to point relation between those arrays. first `MIRROR_REPOS` element is a mirror of `REPOS` element.

## Usage

```bash
./gitMirror
```

if you got permission error you should run this:

```bash
sudo chmod +x ./gitMirror
```

After running script `.repo` directory will create in same directory that bash script exists.
After jobs done you can delete them. but it's better to prevent.
