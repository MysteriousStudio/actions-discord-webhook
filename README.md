# GitHub Actions Discord Webhook

```yaml
    - name: Send status to Discord
      uses: nebularg/actions-discord-webhook@v1
      with:
        webhook_url: ${{ secrets.discord_webhook_url }} # required
        status: ${{ job.status }} # optional, this is the default
      if: always() # or failure() or success()
```

![Discord message](https://raw.githubusercontent.com/nebularg/actions-discord-webhook/master/Screenshot.jpg)
