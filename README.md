# Requirements

* python v2.7
* pip install beautifulsoup4
* pip install requests

# Crawler options

```python
Options:
  --version                             show program's version number and exit
  -h, --help                            show this help message and exit
  -q, --quiet                           enable quiet mode
  -l, --links                           get links for specified url only
  -d DEPTH_LIMIT, --depth=DEPTH_LIMIT   maximum depth to traverse
  -c CONFINE, --confine=CONFINE         confine crawl to specified prefix
  -x EXCLUDE, --exclude=EXCLUDE         exclude URLs by prefix
  -L, --show-links                      output links found
  -u, --show-urls                       output URLs found
  -D, --dot                             output Graphviz dot file
  -p OUT_PATH, --path=OUT_PATH          output path directory
  
Usage: crawler.py [options] <url>

```
# Usage

Save links to file
```bash
python crawler.py -d 0 -u -p "/var/tmp/downloaded/" "https://github.com/"

Crawling https://github.com/ (Max Depth: 0)
Stats:    (2/s after 19.02s)
```

Get all links
```bash
python crawler.py -d 0 -l "https://github.com/"

0. https://github.com/#start-of-content
1. https://github.com/
2. https://github.com/join
3. https://github.com/login
4. https://github.com/explore
5. https://github.com/features
6. https://enterprise.github.com/
7. https://github.com/blog
8. https://help.github.com/terms
9. https://help.github.com/privacy
10. https://github.com/plans
11. https://enterprise.github.com
12. https://github.com/integrations
13. https://central.github.com/mac/latest
14. https://mac.github.com
15. https://windows.github.com/
16. https://github-windows.s3.amazonaws.com/GitHubSetup.exe
17. https://windows.github.com
18. https://mac.github.com/
19. https://status.github.com/
20. https://developer.github.com
21. https://training.github.com
22. https://shop.github.com
23. https://github.com/about
24. https://help.github.com
25. https://github.com
26. https://github.com/site/terms
27. https://github.com/site/privacy
28. https://github.com/security
29. https://github.com/contact
```



