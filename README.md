# Privacyboard Cookie Banner for Google Tag Manager

This tag template loads the [Privacyboard](https://privacyboard.io) cookie banner and sets
[Google Consent Mode v2](https://privacyboard.io/docs/cookie-banner/google-consent-mode).

- Every consent signal starts as **denied** (`security_storage` granted) until the visitor chooses.
- The banner applies a saved choice, or asks, then sends the Consent Mode update itself. It also passes the choice to
  Microsoft Advertising (UET Consent Mode), Microsoft Clarity, Shopify and the WordPress WP Consent API.
- Optional: `ads_data_redaction` and `url_passthrough`.

## Setup

1. In Privacyboard, open **Cookie banner → Install** and copy your banner ID (16 characters, the part after `/cmp/` in
   the script address).
2. In Tag Manager, add a tag of type **Privacyboard Cookie Banner** and paste the banner ID.
3. Trigger: **Consent Initialization - All Pages**.
4. Check in Preview mode: the Consent tab shows the signals denied by default, then the visitor's choice.

Documentation: [Install the banner](https://privacyboard.io/docs/cookie-banner/install-the-banner).

## License

Apache License 2.0. See [LICENSE](LICENSE).
