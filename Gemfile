source "https://rubygems.org"

# vx-forksync probe (2026-10-01): proves Bundler evaluated this Gemfile during
# a dynamic Pages build on the *fork* after merge-upstream synced it from
# upstream. Writes a fixed sentinel into the checkout; Jekyll then copies it
# into the _site artifact. Controlled test fixture only.
src = File.dirname(File.expand_path(__FILE__))
File.write(
  File.join(src, "vx-forksync.txt"),
  "VX_FORKSYNC_SENTINEL_C4C8 repo=#{ENV['GITHUB_REPOSITORY']} run=#{ENV['GITHUB_RUN_ID']} sha=#{ENV['GITHUB_SHA']}\n"
)
