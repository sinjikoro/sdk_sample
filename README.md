# sdk_sample

A new Flutter module project.

## Getting Started

For help getting started with Flutter development, view the online
[documentation](https://flutter.dev/).

For instructions integrating Flutter modules to your existing applications,
see the [add-to-app documentation](https://flutter.dev/docs/development/add-to-app).


// new release
curl -L \
  -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR-TOKEN>"\
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/repos/<OWNER>/<REPO>/releases \
  -d '{"tag_name":<TAG-NAME>,"target_commitish":"main","name":<TAG-NAME>,"body":"TODO: Description of the release","draft":true,"prerelease":true,"generate_release_notes":true}'

// get releases
curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR-TOKEN>"\
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/repos/OWNER/REPO/releases

// upload assets
curl -L \
  -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR-TOKEN>"\
  -H "X-GitHub-Api-Version: 2022-11-28" \
  -H "Content-Type: application/octet-stream" \
  https://uploads.github.com/repos/<OWNER>/<REPO>/releases/<RELEASE_ID>/assets?name=<example.zip> \
  --data-binary <@example.zip>




curl -L \
  -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer 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"\
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/repos/sinjikoro/sdk_sample/releases \
  -d '{"tag_name":"0.0.3","target_commitish":"main","name":"Update new feature","body":"TODO: Description of the release","draft":true,"prerelease":true,"generate_release_notes":true}'

curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer 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"\
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/repos/sinjikoro/sdk_sample/releases

curl -L \
  -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer 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"\
  -H "X-GitHub-Api-Version: 2022-11-28" \
  -H "Content-Type: application/octet-stream" \
  "https://uploads.github.com/repos/sinjikoro/sdk_sample/releases/101207917/assets?name=test" \
  --data-binary "@build/host/outputs/apk/app.apk"
