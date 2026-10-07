# oss-vrp-replica-workflows

Structural **replica**, for authorized security research, of
`google-gh-automation/workflows` → `.github/workflows/github_actions_scan.yml`
at commit `22b63c643fbe7b395b00cc3952ab552decc586c7`
(blob `sha256:6a5870fc3418addfa11105fe32b8d3e44e224b19d26e9d003a0305688b991435`).

It exists only to measure GitHub Actions and OIDC behaviour inside repositories we own.

* It **never** calls Google's reusable workflow; it copies its content.
* Every identity-provider string and bucket name here is **fake**.
* Every `curl` to `storage.googleapis.com` in the original is replaced by `echo`.
* No token is ever exchanged with any identity provider, and no raw token is ever printed.
