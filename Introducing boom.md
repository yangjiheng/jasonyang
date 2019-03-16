# Introducing Boom, rar extracting tool under mac

So far, I haven't really found any easy to use tool to extracting files out of compressed rar files. So far there are a couple tools available in Mac App Store, but most of them are not designed nicely. Also, it's always easier to use a command line tool to do this kind of job rather than a GUI software (right?), so let's go and build one.

Thanks for the almighty github, we almost always don't have to create new wheels. I looked it up, and found UnrarKit, which is very easy to import and develop with, and then half an hour later, the tool is there. After I use it personally for a while, it's stable and easy to use than most extracting tools, so I'm releasing the code publicly and give back to people who is in need. 

Later on, I quit all GUI based software to extracting compressed files, so then I used SSZipArchive to handle zip files, then the console based tool and extract zip files and rar files. So it's all integrated and easy to use.

For boom, the usage is very easy to grasp:

    boom -i inputfile -o outputpath -p password

so you can specify an input compressed file, an output directory for extracted files, and then specify a password if the file is encrypted, then you can wait things done. 

If you need this extracting tool, you can clone code from github and build it locally with XCode and a "boom" tool will be generated. Github address for this project is: https://github.com/yangjiheng/boom. Hope it helps.
