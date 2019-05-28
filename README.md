# TV4Dialog  Corpus

By Leilan Zhang

TV4Dialog is a multi-turn **Chinese** and **English** dialogue corpus, which is constructed based on scripts and subtitles of 4 TV series: *Castle*, *Friends*, *House*, *TBBT*.  This corpus is suited to the fields of dialogue generation, dialogue action analysis and machine translation.

### License

TV4Dialog is a part of contribution of our paper *Automatically Annotate TV Series Subtitles for Dialogue Corpus Construction*. 

The data in this repository is provided under the license [CC BY 2.0](<https://creativecommons.org/licenses/by/2.0/>). Please cite the following paper if you use it: 

> ```
> @inproceedings{zhang2019,
>   title={Automatically Annotate TV Series Subtitles for Dialogue Corpus Construction},
>   author={Leilan Zhang, Qiang Zhou},
>   year={2019},
>   publisher = {{APSIPA} Press},
>   address={Lanzhou, Gansu, China}
> }
> ```

### How it was made

We first collected the English scripts and Chinese-English subtitles of the 4 TV series from the Internet. The scripts were then parsed to XML format with extracted elements like scenes, speakers and utterances. 

As we know, it is hard to judge whether two continuous subtitle lines belong to the same speaker or not because of the lack of obvious marks between them. Using the methods proposed in our paper, we aligned the utterances in scripts to the subtitle lines and annotated the subtitles with speaker tags. According to those annotated tags, we merged the continuous subtitle lines belong to the same speaker to a single utterance.

### Details of TV4Dialog

This corpus is composed of 26w utterances both in Chinese and English. It provides both the scripts (en) and the subtitle (en & zh),  basic statistics are list below:

![](C:\Users\Layland\Documents\projects\myGitHub\TV4Dialog\pics\stat_1.png)

![](C:\Users\Layland\Documents\projects\myGitHub\TV4Dialog\pics\stat_2.png)

**xmlScript** stores the parsed scripts of the 4 TV series in XML format (in English). 

**withSpkr** stores the subtitles annotated with speaker tags and *uid* tags (en & zh parallel).

**extracted** stores the merged utterances extracted from the annotated subtitles (in Chinese).

### Acknowledgments

We would like to thank website [assrt.net](http://assrt.net) for the help of providing the raw subtitle files. 