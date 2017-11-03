This project is based on [Kyubyong's](https://github.com/Kyubyong/transformer) excellent work, thanks for his attempt!
Based on that, we have:
* implement the model under tf.estimator.Estimator API
* add an option to tie the weights between encoder embedding weight and decoder embedding weight, as paper suggests
* add an option to tie the weights between decoder embedding weight and output projection weight, as paper suggests
* more activation choices

>python train.py --hidden_units=128 --num_epochs=30 --num_heads=4 --positional_encoding=learned --tied_proj_weight --tied_embedding --activation=lrelu

The image below (a kind of) illustrates how an army of attentions work:
![alt text](https://github.com/zhedongzheng/finch/blob/master/assets/transform20fps.gif)