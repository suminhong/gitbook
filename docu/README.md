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



python code

```python
import json
import urllib3

SLACK_URL = ""
MESSAGE = "Lambda Trigger Test"

def lambda_handler(event, context):
    
    message = {
        'text': MESSAGE
    }

    http = urllib3.PoolManager()
    response = http.request('POST', SLACK_URL, body=json.dumps(message).encode('utf-8'), headers={'Content-Type': 'application/json'})
    
    if response.status != 200:
        raise ValueError(f'Request failed: {response.data.decode("utf-8")}')

    return {
        'statusCode': 200,
        'body': json.dumps('Slack 메시지가 전송되었습니다!')
    }
```

yaml

````yaml
```yaml
image:
  # image.repository -- Redash image name used for server and worker pods
  repository: redash/redash
  # image.tag -- Redash image [tag](https://hub.docker.com/r/redash/redash/tags)
  tag: 10.0.0.b50363
  # image.pullPolicy - Image pull policy
  pullPolicy: IfNotPresent
```
````

terraform

````
```terraform
resource "aws_kms_key" "this" {
  description = local.tf_desc

  tags = merge(
    local.module_tag,
    {
      Name = local.kms_name,
    }
  )
}
```
````

hcl

````hcl
```terraform
resource "aws_kms_key" "this" {
  description = local.tf_desc

  tags = merge(
    local.module_tag,
    {
      Name = local.kms_name,
    }
  )
}
```
````

