# error-invalidSrc
Server Error:
Error: Invalid src prop {https://yourlink.com} on 'next/image', hostname "your.link.com" is not configured under images in your 'next.config.js' see more info: https://nextjs.org/docs/messages/next-image-unconfigured-host
____________________________________

When you're having this issue... 

simply go to package.json
create a file: next.config.js

inside of that file enter the following:
module.exports = {
    images: {
        domains: ['https://yourlink.com']
    }
}

save it...
then exit out of the server then re-run the dev.
