# Check basic commit message formatting
commit_lint.check warn: :all

# Ensure a clean commits history
if git.commits.any? { |c| c.message =~ /^Merge branch/ }
  warn('Please rebase to get rid of the merge commits in this PR')
end
