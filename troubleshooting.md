# Troubleshooting Log

Record actual issues from your own setup. Do not list hypothetical issues as completed troubleshooting.

## Entry template

| Field | Details |
|---|---|
| Date | [YYYY-MM-DD] |
| Stage | [VirtualBox / Kali installation / GRUB / networking / other] |
| Issue observed | [Describe the exact symptom] |
| Checks performed | [What you inspected] |
| Resolution | [What fixed it, or state unresolved] |
| Verification | [How you confirmed the result] |
| Evidence | [Screenshot filename] |

## Installation note

During the Kali installation, review the installer prompts carefully. For a VirtualBox VM, GRUB is normally installed to the VM's virtual hard disk (commonly `/dev/sda`) rather than an individual partition. Confirm the target shown by your own installer before proceeding.
