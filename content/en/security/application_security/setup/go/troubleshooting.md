---
title: Troubleshooting Go App and API Protection
---

## Common Issues

### No security signals appearing

1. **Verify Agent version**
   - Ensure you're running Datadog Agent v7.41.1 or higher
   - Check Agent status: `datadog-agent status`

2. **Check Go tracer version**
   - Confirm you're using Go tracer v1.53.0 or higher

3. **Verify environment variables**
   - Ensure `DD_APPSEC_ENABLED=true` is set
   - Check `DD_SERVICE` and `DD_ENV` are properly configured

4. **Check file system permissions**
   - Ensure the application has write access to `/tmp` if you are not on linux

### Application fails to start

TODO

### Still having issues?

If you're still experiencing problems:
1. Check the [Application Security Monitoring troubleshooting guide][1]
2. Review the [Java tracer documentation][2]
3. Contact [Datadog support][3]

[1]: /security/application_security/troubleshooting
[2]: /tracing/trace_collection/compatibility/java
[3]: /help
