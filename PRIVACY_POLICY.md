# Arbiter House Privacy Policy

Effective date: 11 October 2026

This policy covers the Arbiter House iPhone and iPad app (bundle identifier `ArbiterHouse`). The app compares language models with your prompt and recommends suitable models. It does not run your prompt on the recommended models.

## Developer and contact

Arbiter House is provided by **Malthe Hertz**. In this policy, “we” means the app developer, responsible for the app's processing described below.

For privacy questions or requests, email [ivy.barlow9617@gmail.com](mailto:ivy.barlow9617@gmail.com). Please avoid including sensitive prompts in your message.

## Data kept on your device

Arbiter House saves the following in its local app storage:

- Your current prompt draft.
- Your latest **100 runs with saved scores**, including incomplete comparisons. Records contain the full original prompt, the excerpt sent for scoring, model scores and descriptions, timestamps, and information needed to identify the catalog and scoring version.
- Progress checkpoints and batch information needed to continue an interrupted comparison.

The original prompt remains in local history even if only a shortened excerpt was sent. New saved runs replace older history entries beyond the 100-run limit. Drafts and checkpoints remain until replaced or cleared. Saved results can be opened offline; doing so does not submit another evaluation. Editing or reusing a prompt does not itself send it to the scoring service.

These files use iOS file protection and are marked as excluded from backups. We do not provide cloud history synchronization or a server copy of your local history. The model catalog and logos are bundled with the app; browsing them does not send your prompt to OpenRouter or to the listed model providers.

## When information leaves your device

Selecting **Find my model**, **Retry remaining models**, or **Continue** starts or resumes remote scoring. The app sends HTTPS requests to `https://api.typesafe.pro/v1/systemone`, an independent gateway that forwards evaluations to **TypeSafe AI, Inc.** at `api.typesafe.ai`.

Requests contain your prompt or its shortened excerpt, the candidate models' IDs, names and descriptions, scoring instructions and criteria, question identifiers, and the evaluator model/version. A comparison uses multiple batches, so the same excerpt is transmitted more than once. Automatic retries may resend a batch. If the service rejects a request as too large, the app can shorten the excerpt further and restart the comparison.

For long prompts, the app removes a middle section while retaining the beginning and end. This is a size limit, **not anonymization or sensitive-data removal**. Anything you include in the transmitted text may be processed remotely. Do not submit passwords, API keys, confidential material, or personal information you are not entitled to share.

No app account or user API key is required. However, network requests are not anonymous in the sense of being untraceable: the gateway and network infrastructure receive connection information such as your IP address and standard request metadata.

## Gateway and upstream processing

The gateway operator's [published TypeSafe app privacy policy](https://github.com/e-eugene/TypeSafe-ios/blob/main/PRIVACY_POLICY.md) identifies **NEXABRIDGE LTD** and describes its gateway practices. It reports that request bodies and successful answers are not saved in its application database, while operational records include IP addresses, request identifiers, times, routes, status/error codes, sizes, timings, and token usage. Diagnostics can contain upstream error excerpts that may echo submitted content.

That policy describes seven-day expiry for activity and database error records, with periodic cleanup, and separate diagnostic logs that rotate by size. These are the gateway operator's stated practices, not a guarantee that all copies disappear after seven days. Local deletion in Arbiter House does not control those records.

TypeSafe AI's [Privacy Policy](https://typesafe.ai/legal/privacy-policy) states that its services are hosted in the United States and that submitted input is not used to train or fine-tune models. It also provides for retention to support its services, business purposes, and legal obligations, without one fixed period for all API data. **Scoring is not a zero-retention service.**

Providers may use hosting, security, and other service providers, and may disclose information as required by law. Processing may take place outside your country. TypeSafe AI's [Data Processing Addendum](https://typesafe.ai/legal/data-processing) describes its contractual processing terms and international-transfer safeguards. Contact us for information about the safeguards applicable to your request.

## Purposes and legal bases

We process submitted information to provide the comparison you request. Where applicable data-protection law requires a legal basis, this processing is necessary to perform the service contract with you. Providing a prompt is optional, but fresh scoring cannot work without sending the evaluation request.

We use support correspondence to answer questions and resolve problems, based on our legitimate interests in supporting the app. Security, abuse prevention, and troubleshooting also serve legitimate interests; information may additionally be processed where required by law. Providers describe their own processing purposes in their policies. We do not sell personal information or use the app for targeted advertising.

The rankings are recommendations for your own choice of software. The app does not use them to make legal or similarly significant decisions about you.

## Deletion and cancellation

You can delete individual saved runs in **History**. **Clear** in the prompt screen starts a fresh draft but keeps saved history. To remove drafts, saved requests, results, and checkpoints together, use **Settings → Clear all local data** and confirm. Deleting the app and its data also removes its local records; merely offloading the app may retain data.

Cancel stops unfinished work and keeps scores already received so you can continue later. Backgrounding pauses unfinished work and saves progress. Neither cancellation nor clearing local data can retract requests already received by a server or guarantee that remote processing stops. Contact us about server-side privacy requests; they are separate from the app's deletion controls.

## Other information and services

The app contains no advertising, tracking, or third-party analytics SDKs. It does not request access to your contacts, location, camera, microphone, photos, or health data. Copying a model ID uses the system clipboard only when you select that action.

If you email us, we receive your email address, message, and any attachments. We retain support correspondence only as needed to address the matter, related disputes, and legal obligations. GitHub issues are public: do not post private prompts or personal information there.

If you test a beta through TestFlight, Apple collects and shares testing information with the developer, including crash logs, usage information, and feedback, under [TestFlight & Privacy](https://www.apple.com/legal/privacy/data/en/test-flight/). We use that information to diagnose problems and improve the app, and retain it only as needed for those purposes and legal obligations. Apple controls its own retention. External websites opened from the app or this policy have their own privacy practices.

## Your rights

Depending on your location and applicable law, you may request access, correction, deletion, restriction, or portability, and object to processing based on legitimate interests. Send requests or privacy complaints to [ivy.barlow9617@gmail.com](mailto:ivy.barlow9617@gmail.com). We may need limited information to verify your request and locate relevant records. An approximate request time is more useful than resending sensitive content. We cannot retrieve drafts stored only on your device.

You may also complain to your local data-protection authority, including the [UK Information Commissioner's Office](https://ico.org.uk/make-a-complaint/) where applicable. Rights can be subject to lawful exceptions; records may already have expired.

## Children and changes

Arbiter House is not directed at children. TypeSafe AI states that its services are not directed to people under 18. Do not submit children's personal information. Contact us if you believe such information has been submitted.

We will publish updates in this document and change its effective date when our practices change.
