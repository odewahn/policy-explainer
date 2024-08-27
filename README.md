```
init
load --fn=source/ai-policy.txt
prompt --task=tasks/010-pdftext-to-markdown.jinja
transfer-prompts --to=blocks --group_tag=source
prompt --task=tasks/020-interview.jinja --persona=personas/screenwriter.txt
```
