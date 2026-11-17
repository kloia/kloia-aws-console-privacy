# Kloia AWS Console: privacy policy

Last updated: 17 November 2026

Kloia AWS Console is a browser extension published by kloia for kloia employees. It opens the
AWS Management Console for AWS accounts that the signed-in employee is entitled to through
kloia's AWS IAM Identity Center. It is not available to the public.

## What the extension handles

- **Your work email address.** AWS IAM Identity Center returns it when you sign in. The
  extension shows it in its window and uses it as the AWS session name when it opens an AWS
  console, so the AWS account's own audit log records who signed in.
- **An AWS IAM Identity Center access token.** It is kept in the browser's session storage,
  in memory only, and is deleted when the browser closes or when you sign out. It expires
  after at most 8 hours.
- **Short-lived AWS credentials.** They are requested when you open a console, used once to
  create the console sign-in, and discarded. They are never stored.
- **The list of AWS accounts you can reach.** It is read from AWS IAM Identity Center and
  from kloia's account catalogue in AWS, and kept in memory while the browser is open.
- **Your preferences and the profiles you add yourself** (filter, role choices, appearance,
  custom profiles). They are kept in your browser's synced extension storage. They contain no
  credentials.

## Where data goes

The extension sends requests only to Amazon Web Services: AWS IAM Identity Center, AWS STS,
Amazon S3 (kloia's account catalogue) and the AWS console sign-in service. It does not send
data to kloia's servers or to any other party, and it contains no analytics, advertising or
tracking.

## What kloia does not do

kloia does not sell or transfer this data to third parties, does not use it for any purpose
other than opening AWS consoles and producing AWS CLI configuration for the signed-in
employee, and does not use it to determine creditworthiness or for lending.

## Your choices

Signing out in the extension deletes the access token. Removing the extension deletes all of
its data from the browser. Access to AWS accounts itself is managed by kloia's access process,
not by this extension.

## Contact

Questions about this policy: sre@kloia.com.
