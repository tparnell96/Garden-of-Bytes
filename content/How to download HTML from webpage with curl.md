
## The curl and the wget commands make it easy to download content from web sites.

One of the most versatile tools for collecting data from a server is **curl**. The “url” portion of the name properly suggests that the command is built to locate data through the URL (uniform resource locater) that you provide. And it doesn’t just communicate with web servers. It supports a wide variety of protocols. This includes HTTP, HTTPS, FTP, FTPS, SCP, SFTP and more. The **wget** command, though similar in some ways to **curl**, primarily supports HTTP and FTP protocols.

### Using the curl command

You might use the **curl** command to:

- Download files from the internet
- Run tests to ensure that the remote server is doing what is expected
- Do some debugging on various problems
- Log errors for later analysis
- Back up important files from the server

Probably the most obvious thing to do with the **curl** command is to download a page from a web site for review on the command line. To do this, just enter “curl” followed by the URL of the web site like this (the content below is truncated):

```curl https://www.networkworld.com/category/linux/```

You’ll see some timing data plus the content. To save the content to a file, redirect the output to a file using a command like this:

```curl https://www.networkworld.com/category/linux/ > linux.html```

The downloaded file can then be viewed on your system using **cat** or **more** to see the html content or a browser to view the web page.