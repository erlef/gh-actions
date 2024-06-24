# erlef/gh-actions/stable/removal-acking

Requires a user to acknowledge the removal of a given Action.

## References

### Usage

```yaml
# action.yml
inputs:
  # Add the acknowledgement of the removal input
  removal-acknowledged:
    description: The action removal has been acknowledged
    required: true
    default: false

runs:
  using: composite
  steps:
    - name: Verify Removal Acknowledgement
      uses: erlef/gh-actions/stable/removal-acking@v0.1.0
      with:
        action-name: erlef/gh-actions/preview/myactioname
        requires-ack: true
        removal-reason: Action migrated to stable
        removal-date: 2024-07-22
        # Pass the removal acknowledgement input
        user-ack: ${{ inputs.removal-acknowledged }}
```
