curl -s "https://api.github.com/repos/Prathamashastryc/File-Storage/contents/sort?ref=main" | grep -o '"download_url": *"[^"]*"' | cut -d'"' -f4 | xargs -n1 curl -fLO
