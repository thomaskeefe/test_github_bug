# Minimal reproducible example of GitHub bug

The following bug concerns relative links in READMEs (such as this README.)

On branch `master`, this README has no images. On `development`, it does have an image, which is a relative link to an image in the repository, (however, only on `development`).

There is an open PR to pull development into `master`. In the Files Changed tab of the PR, the rich diff for README.md shows that there should be an image, howver the link is broken (because the image file doesn't exist in `master`.)

If you click on broken image though, you get taken to the correct image on the `development` branch.

When you then press Back in the browser, you return to the rich diff, but now the image appears as it 'should'.

The bug is that the image does not show up in the rich diff unless you do this.
