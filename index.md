# Settings


## Bitbucket access

To access Bitbucket, you have to set environment variables. You have these options:

- Set up a username and password as `BITBUCKET_USER` and `BITBUCKET_PASSWORD`;
- Set up `BITBUCKET_TOKEN` (see below).

### Bitbucket Access Token

<div id="access_token_wrapper" style="display:none" class="attention">
  <p>You already have authorized Arche.</p>
  <p>Copy the code below and assign it to <code>BITBUCKET_TOKEN</code> environment variable.</p>
  <input id="access_token" style="width:94%;padding:1%" type="text" />
</div>

<script defer>
    if (window.location.hash) {
      var params = new URLSearchParams(window.location.hash.replace(/^#/, ''))
      var token = params.get('access_token')
      if (token) {
          document.querySelector('#access_token').value = token;
          document.querySelector('#access_token_wrapper').style.display = 'block';
      }
  }
</script>

You can [click here to authorize Arche, or to get fresher token](https://bitbucket.org/site/oauth2/authorize?client_id=MKCfX5xkXHbdRPYwKa&response_type=token).