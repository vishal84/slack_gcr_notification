# slack_gcr_notification

Notify via a message in Slack when a GCR build is complete by subscribing to pub/sub topic.

Create Google Cloud Storage Bucket: \r
gsutil mb gs://[STAGING_BUCKET_NAME]

Create Google Cloud Function: \r
gcloud beta functions deploy subscribe --stage-bucket [STAGING_BUCKET_NAME] --trigger-topic cloud-builds
