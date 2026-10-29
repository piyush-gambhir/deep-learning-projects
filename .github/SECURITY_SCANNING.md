# Security scanning

Ruff 0.17.3 checks notebook Python security rules without executing cells. GitHub secret
scanning remains enabled for recognized provider credentials.

The chatbot's `oov_token="<unk>"` is an NLP vocabulary marker, not a credential. Its single
`S106` false positive is annotated at that call site. Do not use that exception for API keys.
