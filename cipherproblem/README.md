# Cipher problem

## Brief

Imagine you are working in the communications department for a major bookstore, "EarthRocks." You've been intercepting communications from your biggest rival, "WindPebbles," but suddenly you can't read their messages!

## Stage 1

You know they must be up to something big, and you've been tasked with uncovering their secrets. Upon investigation, you discover they are using a Vigenère cipher for their inter-department messages, employing a shared key—the scoundrels! This works by shifting the letters by a key, where A=1, B=2 etc. An example of how this works is shown below: 

```
INPUT TEXT:     hello world
KEY:            abcdef
OUTPUT TEXT:    igopt cptoh
```

You have the following messages to decipher, and you're hopeful that solving these will lead you to further information: 

> dti scrz:ogpg lna, ewgphp pdip qjg yqgbln rdxojctepitqch njpcyga wlu qtpp razuts.

> umi xtkz:vkwb dhe dd, ittqlm tdlcgu rwj qixao mpt fkmkyhchbr lxivchixl ryipth mw pdr utilivul.

> tju lshl:edq nikxbkwx tlgzmh zfwi s xvmlfcpw pfc, lmjw ax gmfj us bztx tj b washpw jokdntl otsh.

> vff mudw:ybf wjs xuqf cq glpmiwbey cofjlomq np fmy cgxcoqxm ta jpfddioq huo othuusof itllusa be ybfk flf.

> utf dfvz:yafglteqx, ita kbgep fghiaw rdg wwx aakpbcs btk xe btng lawh uaqw.

A co-worker has solved a few before and has suggested to you that the keys tend to be English words. We suspect they are likely using words from their most popular dictionaries. We've got our hands on a copy for you—take a look at dictionary.txt.

## Stage 2

Great job cracking the first messages! However, it seems WindPebbles have realised you're onto them. The next few messages we have received appear to have more complex keys, this time made up of several words.

Can you solve these? Time is of the essence; we need to crack these messages quickly!

> mcuff lbhmlm:nu ktp yzy jjth hc yagmx, jh pxx lbm bpflq tx nqrfg, bq bsm bmf ozb tx qqxecf, fy oua yis tdj gz ntpzbpmfyax, jh pxx lbm jqcve tx vmqjsy, fy oua yis xmtub wk jbvojvotnum, bq bsm bmf gxxxgh wk mwzey, an eft hab xwuato cy afjevjtg, bq bsm bmf gionfa wk icib, nl qix uvx tnfnmw pt wbxhuqw, xs axi wpmwzhafsy vmkpfx rx, oy pfe bhqmaho gfthoj mm, ej xskb fdf otjbz anjyky uc abfnyv, bf kxoj sft lpwgd ialmhu hab tlbmw xor.

> loqwl lblozx:cu oul x klqzbu uiea mug bh bhlbi, jhl mbf ufhztm exlf knkftcvz nialmbnh.

> mcusm fghmxt:el. zor qla. iimfnjq, uu folcsv zwzf, kekawz sjcuf, kilm ufjhf yg ypq ngbh xbmd kzeg uwxuwwsmm rizrog, gjffq ngo uffc gchv. he. fzjyaws lbri xznzgf. jj ogh s vhh, piynd ava ynln wslcmm ehg ssxx, cqlndmag is hcl moqr c awxn duqhs qicxhvpjj. exh. voqtzis efg ouks sts tfnori uvi vvq vbait lbd vgyut fajhpy gl cwwj, xvmwp hohr ks nkgq orftyf ix gcr uuwti ki lvql in msm gkrw yeqcmh cr npj bzvimtujjm. sis hozxzzlu msj p kgzmz wiv hogygi vasdyx bbh cv yvzvt thocaim uvilm bon aq kattj vnz orsemsmr. owk jjjmkfm lul f gdfvjj ipdfde zmfg ucoggw. knt shc isv bcxpvaf osstk jnuhil pfr v fqs ugadyc iovlg ucoggw. lntq fhwsh ziw tmbo yzk smlrmscm isr yvf sgz hhyzl hs npja hhem. lntq xhe bsn ojh vyqsy.

> xitxo bykzfi:bk j bwqs mg qqy owcyga cbmws pbsnx i mcfufc. hwy o rtpcs, lnfxr, tnn ptzi, yfufmi kmme cbm jbhl lo qwwaw tkm uv tcdr pvytq, bsk vnn i ifc, uxay, afbhr exfm bwxa kxnpnbk bk rn bt gmm axqv tb sk bjn: qy kel x qijgwx-aluy, isr xaxc gmfbw vlvzwwh.

> tikrt xwwrgf:wi gjj tydxobdai yzy rcjjzeuj oup rssvggi. lbfh ioy zciw gxcz dzbrqw pbgz oittd sha wbg wrgs ocatmm mrifjxbs bg v oci eist.
