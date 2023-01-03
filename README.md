# GitHub Actions with Writerside

This repository contains an example GitHub Actions workflow configuration that builds a Writerside project and produces .zip archive with static HTMLs.
Use the image `registry.jetbrains.team/p/writerside/builder/writerside-builder:2.1.984` and call

`/opt/builder/bin/idea.sh helpbuilderinspect -source-dir . -product $PRODUCT -output-dir artifacts/ || true`


The $PRODUCT should be name_of_module / product_id so in our example it is help_module/d.
This will generate a zip archive with the built web pages. The name of the archive is webHelpX2-all.zip where X gets replaced by the product id in caps.
See the blank.yml file on Actions tab for an example in full context.