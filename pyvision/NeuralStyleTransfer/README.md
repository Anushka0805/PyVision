## Neural Style Transfer: An implementation of the paper "A Neural Algorithm of Artistic Style".

Link to the paper: https://arxiv.org/pdf/1508.06576.pdf

The idea is to extract the _content_ from one image, the 'content image', and the _style_ or _texture_ from another image, the 'style image', to get a single output which has a combination of the two.

## Here are some of the results
Output Images:
![](/output/content1+style6.png)


## Steps required to run:

from pyvision.NeuralStyleTransfer.neural_style import Neural_Style

style_img, content_img = ('path_to_style_image', 'path_to_content_image')

nst=Neural_Style(num_steps=300)

output = nst.run_style_transfer(style_img, content_img)

nst.imshow(output)
