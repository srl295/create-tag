
# Create a Tag

This action simply calls the GitHub API to create a tag.

## Example Use

The following will tag a specific sha with the tag `my-tag`.

```yaml
 - name: Tag Commit
   uses: simpleactions/create-tag@d5c32a2d86b1f96142bbe1ebe8b3b62b0a0587ff
   with:
     sha: 0e33f857188318c640a851710a554c071b464975
     tag: "my-tag"
     message: "Deployed via GitHub by @${{ github.actor }}"
   env:
     GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
