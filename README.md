# Апелляции на Бана AmSerg Games

## Blocking users

Users that spam requests can be blocked by creating an environment variable called `BLOCKED_USERS`, which should contain a comma-separated list of quoted user IDs. To do this:

1. On your [Netlify dashboard](https://app.netlify.com), click **Deploys** and navigate to **Deploy settings**, and then to the **Environment** option.

2. Under **Environment variables**, click **Edit variables**.

3. Right-click on any mention of the user you want to block, and click **Copy ID**. You need developer mode enabled for this option to show up, see instructions above.

4. Click **New variable**, and create an environment variable with `BLOCKED_USERS` as its key. For the value, paste the user ID you copied in the previous step.
   ![](https://i.imgur.com/5hGRufC.png)

5. To add more IDs, add a comma after the first quoted ID, and then repeat these steps starting from step 3.
   ![](https://i.imgur.com/jNKgS2B.png)

6. Redeploy the site with **Deploys** -> **Trigger deploy** -> **Deploy site**.
