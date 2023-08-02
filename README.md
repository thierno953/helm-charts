# Helm 

```bash
# helm create demochart
helm create ui-deploy

# Verify the Conversion of YAMLs
helm template dev-templ -f ./ui-deploy/values-dev.yaml ./ui-deploy --debug
helm template dev-templ -f ./ui-deploy/values-dev.yaml ./ui-deploy --debug > dev.yaml
helm template dev-templ -f ./ui-deploy/values-qa.yaml ./ui-deploy --debug > qa.yaml
helm template dev-templ -f ./ui-deploy/values-prod.yaml ./ui-deploy --debug > prod.yaml
```
