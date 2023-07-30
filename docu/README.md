---
description: dskf'sfksd
---

# 😅 Home

jshdfksdjf



sdkjfhsdkjf



$$f(x) = x * e^{2 pi i \xi x}$$sdsf



```
prompt_kubectx () {
  if [[ $(kubectx -c) == *"prod"* ]]; then
    prompt_segment bg red $(kubectx -c)%{% raw %}
{%F{white}%}:%{%F{cyan}%}$(kubens -c)
  else
    prompt_segment bg yellow $(kubectx -c)%{%F{white}%}:%{%F{cyan}%}
{% endraw %}$(kubens -c)
  fi
}
```
