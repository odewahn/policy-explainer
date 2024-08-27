This repo converts our AI policy into an audio dialog format:

- Source is in source/ai-policy.txt. This is just copied from the original AI policy document and pasted into a text editor.
- Tasks are in tasks

```
init
load --fn=source/ai-policy.txt
prompt --task=tasks/010-pdftext-to-markdown.jinja
transfer-prompts --to=blocks --group_tag=source
prompt --task=tasks/020-interview.jinja --persona=personas/screenwriter.txt
```
