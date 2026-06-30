# Risk Register

| Risk | Impact | Likelihood | Mitigation |
|---|---|---|---|
| Hallucinated answers | Incorrect troubleshooting guidance | Medium | Use citations and require source-grounded answers |
| Poor retrieval quality | User receives irrelevant answers | Medium | Tune chunk size and evaluate Recall@5 |
| Sensitive data exposure | Security/compliance concern | High | Use only sample or sanitized data |
| Over-scoped MVP | Delayed delivery | Medium | Keep MVP limited to upload, ask, answer, summarize |
| High API cost | Expensive usage | Low | Start with small sample documents |
| Slow response time | Poor user experience | Medium | Limit retrieved chunks and optimize document size |
| Outdated documentation | Wrong recommendations | Medium | Add document date metadata and re-indexing plan |
