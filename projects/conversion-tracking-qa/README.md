# Conversion Tracking QA

A practical checklist for validating whether marketing conversions are captured, classified, and sent to the right platforms.

## Measurement path

```text
User Action
    ↓
Website / Form / Call
    ↓
GTM
    ↓
GA4 Event
    ↓
Google Ads Conversion
    ↓
Optimization Signal
```

## QA checklist

### Website
- [ ] Correct interaction fires
- [ ] Thank-you / success state is reliable
- [ ] Duplicate submissions are controlled
- [ ] Important parameters are available

### GTM
- [ ] Trigger fires only when intended
- [ ] Variables contain expected values
- [ ] Tags fire once
- [ ] Consent behavior is understood
- [ ] Debug / Preview evidence captured

### GA4
- [ ] Event name is intentional
- [ ] Event parameters are correct
- [ ] Key event configuration is correct
- [ ] Internal/test traffic is handled appropriately

### Google Ads
- [ ] Correct conversion action is used
- [ ] Primary/secondary classification is intentional
- [ ] Attribution and counting settings fit the business
- [ ] Conversion value is configured when meaningful

## QA evidence

For every important conversion, document:

```text
Event → Trigger → Tag → Platform → Status → Evidence → Notes
```

## Common failure modes

- Form submits but conversion tag never fires
- Duplicate conversion firing
- Wrong event marked as primary
- Cross-domain flow breaks attribution
- Phone-click tracking without meaningful lead qualification
- GA4 event exists but Google Ads optimization signal is wrong

> Never expose client credentials, personal data, or confidential campaign information in this repository.
