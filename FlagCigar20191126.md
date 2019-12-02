Explain BAM FLAG value： 143= 1+2+4+8+128 含义：PE read，正常比对，该read没有比对到参考序列，PE序列的另一个配对read没有比对到参考序列，它是PE read2.read paired (0x1) read mapped in proper pair (0x2) read unmapped (0x4) mate unmapped (0x8) second in pair (0x80)
Explain BAM FLAG value： 99=1+2+32+64 含义：PE read，正常比对上序列，它的另一条配对read反向互补后比对到参考序列，它是read1。 read paired (0x1) read mapped in proper pair (0x2) mate reverse strand (0x20) first in pair (0x40)
Explain BAM FLAG value：516=4+512 含义：低于（测序平台）过滤阈值，并且该read没有比对到参考序列 read unmapped (0x4) read fails platform/vendor quality checks (0x200)
Explain BAM FLAG value： 2064=16+2048 含义：反向互补后比对到参考序列（比对到负链），这条read可能存在嵌合，这个比对的部分只是来自其中的一部分序列。 read reverse strand (0x10) supplementary alignment (0x800)
Explain BAM FLAG value： 147=1+2+16+128 含义：PE read 正常比对，反向互补后比对到参考序列，它是PE read2. read paired (0x1) read mapped in proper pair (0x2) read reverse strand (0x10) second in pair (0x80)
Explain BAM CIGAR：14M2D31M 含义：这条序列与参考基因组相比，前14bp能够比对上，中间有2bp的删除，最后有31bp的比对。
Explain BAM CIGAR：3S6M1D5M ： 含义：比对的时候这条read开头的3bp被跳过了，紧接其后的6bp则比对上了，之后有1bp 的删除，最后5bp序列比对上。
Explain BAM CIGAR: 6M14N5M： 含义：比对的时候这条read开头6bp的比对上，之后有14bp跳过参考序列，5bp比对上。
Explain BAM CIGAR: 7M5D8M2I14M (小写：7m5d8m2i14m） 含义：这条序列与参考基因组相比前7bp比对上中间有之后5bp删除delete随后又有8bp比对上，接下来2bp插入，最后14bp比对上。
how long is the read with alignment CIGAR of 7M5D8M2I14M? the long of 7M5D8M2I14M:31
