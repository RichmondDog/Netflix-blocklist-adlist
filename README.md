# Netflix Blocklist for Pi-hole

This is a ready-made blocklist for [Pi-hole](https://pi-hole.net/) designed to block access to Netflix on all devices in your home network.

## What is this for?

If you want to stop devices on your network from accessing Netflix (for example, for parental control), you can use this list with your Pi-hole installation.  
It’s easy to use and you don’t need to be a technical expert.

## How do I use this blocklist?

1. **Copy the Raw Link:**
   - Click on the `netflix-adlist.txt` file in this repository.
   - Click the **Raw** button.
   - Copy the link from your browser’s address bar.

2. **Add the List to Pi-hole:**
   - Open your Pi-hole web interface.
   - Go to **Group Management** > **Adlists**.
   - Paste the link you copied into the **Address** box.
   - Click **Add**.

3. **Update Pi-hole:**
   - In the Pi-hole web interface, click **Update Gravity** (or run `pihole -g` in the terminal).
   - This applies the new blocklist.

4. **You’re Done!**
   - Netflix should now be blocked on all devices using your network’s Pi-hole.

## What does this block?

This list includes the main domains used by Netflix for:
- The website
- Streaming services
- Content delivery (CDN)
- APIs and services

It is designed to block Netflix streaming and access to the Netflix website as completely as possible.

## Can I unblock Netflix later?

Yes.  
Just remove this adlist from Pi-hole’s **Adlists** section and update gravity again.  
Netflix access will be restored.

## Who maintains this list?

This list is maintained by the community.  
If you find a Netflix domain that isn’t blocked, or if you have suggestions, please open an issue or submit a pull request.
