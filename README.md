# Case Assessment Tool

Source of record for the Case Assessment form's custom code. This repo only stores the code. It is not built or deployed from here. To change the live form, edit the file here, then paste it into the form builder.

## Files

| File | Where it goes in the form builder |
|---|---|
| `src/custom-code-element.html` | Custom code element (form markup + live calculator panel) |
| `src/footer-tracking-code.html` | Footer tracking code (conditional logic, damage calculator, URL prefill, Pabbly webhook submit). Not added yet. |

## Notes

- The footer script reads from and writes to element IDs in the custom code element, so if you rename an ID in one file, rename it in the other.
- The footer script posts submissions to a Pabbly Connect webhook. The webhook URL lives in that script, so keep this repo private.
