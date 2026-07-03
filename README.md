# Chargeback Reason Codes (open dataset)

A free, open dataset of all 64 active chargeback reason codes across the four major card networks (Visa, Mastercard, American Express, Discover). Each row has the code, the network, a plain-English meaning, the response deadline, the evidence that supports a rebuttal, a winnability label, and the source document.

## Files
- `chargeback-reason-codes.csv` — the dataset as CSV
- `chargeback-reason-codes.json` — the same data as JSON

## Schema
One row per code: `network, code, title, plain_english_meaning, response_deadline, key_evidence, winnability_label, source`

## Counts
64 active codes: American Express 23, Visa 20, Mastercard 11, Discover 10. Retired codes are deliberately excluded.

## Notes and limitations
The winnability and evidence fields are a synthesis from the network documents plus experience, not official network guidance, so treat them as a starting point. Deadlines are the standard windows; your processor (Stripe, Adyen, and others) often imposes a shorter one. Networks revise codes periodically, so this is a snapshot.

## License
CC BY 4.0. Free to use, cite, or redistribute with attribution.

## Source
Maintained alongside the browsable version at https://chargebackkit.app/reason-codes/ (also on Hugging Face and Kaggle).
