Install hugo
------------------------

curl -s https://api.github.com/repos/gohugoio/hugo/releases/latest \
 | grep  browser_download_url \
 | grep Linux-64bit.deb \
 | grep -v extended \
 | cut -d '"' -f 4 \
 | wget -i -

sudo dpkg -i hugo*_Linux-64bit.deb

Develop
------------------------

git clone git@github.com:eduardoarandah/jero.git && cd jero

hugo server -D


Commands
------------------------

## new post

hugo new posts/my-first-post.md

theme
------------------------

https://themes.gohugo.io/
