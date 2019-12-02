1. Explain BAM FLAG value： 143
143=128+8+4+2+1=10001111
两条read都没有比对到参考序列上。

2. Explain BAM FLAG value： 99
99=64+32+2+1=1100011
第一条read和参考序列完全匹配，第二条read比对到参考序列负链上。

3. Explain BAM FLAG value：516
516=512+4=1000000100
该read没有通过质量控制，没有比对到参考序列上。

4. Explain BAM FLAG value： 2064
2064=2048+16=100000010000
补充匹配的read比对到参考序列的负链

5. Explain BAM FLAG value： 147
147=128+16+2+1=10010011
第二条read比对到参考序列的负链，与参考序列完全匹配。

Question 6-10： BAM CIGAR
6. Explain BAM CIGAR：14M2D31M
在比对的时候这条read开头的14bp比对上了参考序列，接着的2bp序列删除，然后的31bp比对上了参考序列。

7. Explain BAM CIGAR：3S6M1D5M
在比对的时候这条read开头的3bp被跳过，接着的6bp比对上了参考序列，然后接着的1bp序列删除，最后的5bp比对上了参考序列。

8. Explain BAM CIGAR: 6M14N5M
在比对的时候这条read开头的6bp比对上了参考序列，接着的14bp被跳过，然后的5bp比对上了参考序列。

9. Explain BAM CIGAR: 7M5D8M2I14M  (小写：7m5d8m2i14m）
在比对的时候这条read开头的7bp比对上了参考序列，接着的5bp序列删除，然后接着的8bp比对上了参考序列，然后接着的2bp序列插入，最后的14bp比对上了参考序列。

10. how long is the read with alignment CIGAR of 7M5D8M2I14M?
29bp







