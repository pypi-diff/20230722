# Comparing `tmp/gymnasium_minigrid-0.0.4.tar.gz` & `tmp/gymnasium_minigrid-0.0.5.tar.gz`

```diff
@@ -0,0 +1,394 @@
+00000000: 1f8b 0808 dcf5 bb64 02ff 6779 6d6e 6173  .......d..gymnas
+00000010: 6975 6d5f 6d69 6e69 6772 6964 2d30 2e30  ium_minigrid-0.0
+00000020: 2e35 2e74 6172 00ed 3d6b 6fdb 36d7 fd1c  .5.tar..=ko.6...
+00000030: 20ff 8175 8137 76a7 c8f7 3809 e6e1 4953   ..u.7v...8...IS
+00000040: b735 9638 4192 ae0b 8ac2 9565 dad6 aadb  .5.8A......e....
+00000050: 4429 8937 3cff fd3d 87a4 6449 969d 4bd3  D).7<..=..dI..K.
+00000060: 6c4f 4b62 4b2d 913c 3c3c e4b9 9222 f5aa  lOKbK-.<<<..."..
+00000070: 5efd cfa9 71f3 8e1a 631a 3cfb 26a9 26d2  ^...q...c.<.&.&.
+00000080: aa7f 6bb5 6673 f11b dfd7 6b8d 7afd 19b9  ..k.fs....k.z...
+00000090: 79f6 0429 62a1 1140 f3cf 7ecc d4e8 1027  y..)b..@..~....'
+000000a0: b41c daad efec c140 ec75 3a0d bdb3 db6c  .......@.u:....l
+000000b0: edb6 379e a9f4 fda7 e9dc 710d 6645 ced0  ..7.......q.fE..
+000000c0: b15c 6b1a 58e3 ed9a 5ed3 dbd5 47e6 ff4e  .\k.X...^...G..N
+000000d0: a7b3 9aff f3bf eb8d 66ad f18c b415 ff7f  ........f.......
+000000e0: f3a4 ff1b e47f 6367 59fe 3795 fc7f 12f9  ......cgY.7.....
+000000f0: df48 e4ff ee5e 67af 56af efea 3525 fa95  .H...^g.V...5%..
+00000100: fc3f ea1f f606 e7bd c7e2 ff9d 9d9d 55fc  .?............U.
+00000110: dfa8 d7f2 f65f b309 af48 4df1 ff37 4fc7  ....._...HM..7O.
+00000120: fd0b 7264 99d4 6574 7363 73e3 d0f3 e781  ..rd..etscs.....
+00000130: 359d 85a4 6c56 48a3 d668 92a3 c834 1879  5...lVH..h...4.y
+00000140: 4583 d0b3 0d2c 734a 03c7 62cc f25c 6231  E....,sJ..b..\b1
+00000150: 32a3 011d cdc9 3430 dc90 8e35 3209 2825  2.....40...52.(%
+00000160: de84 9833 2398 528d 841e 31dc 39f1 69c0  ...3#.R...1.9.i.
+00000170: a082 370a 0d98 67ee 9418 c484 b636 37a0  ..7...g......67.
+00000180: 6838 0338 cc9b 84d7 4640 a1f4 9818 8c79  h8.8....F@.....y
+00000190: a665 0040 32f6 ccc8 a16e 6884 d8e0 c4b2  .e.@2....nh.....
+000001a0: 2923 e570 4649 e95c d628 5578 2b63 6ad8  )#.pFI.\.(Ux+cj.
+000001b0: 9b1b 964b 3033 ce23 d756 38f3 a290 0494  ...K03.#.V8.....
+000001c0: 8581 6522 108d 58ae 6947 63c4 22ce b62d  ..e"..X.iGc."..-
+000001d0: c792 4d60 754e 02b6 b901 6023 069d 4054  ..M`uN....`#..@T
+000001e0: 35e2 7863 6b82 ff52 de33 3f1a d916 9b69  5.xck..R.3?....i
+000001f0: 646c 21ec 5114 c24b 862f 3939 35ec 49d5  dl!.Q..K./995.I.
+00000200: 0b08 a336 2006 202c 409d 7777 811f 2f84  ...6 . ,@.ww../.
+00000210: d8fb 48d4 5092 89e1 9beb 99e7 64fb 6201  ..H.P.......d.b.
+00000220: 4693 2870 a151 ca2b 8d3d 201b 6ff3 0f6a  F.(p.Q.+.= .o..j
+00000230: 86f8 06cb 4f3c dbf6 aeb1 77a6 e78e 2dec  ....O<....w...-.
+00000240: 14db c781 bb80 4c63 e45d 51de 1f31 ccae  ......Lc.]Q..1..
+00000250: 1702 ba02 0b1c 067f 31b8 328b cd0c db26  ........1.2....&
+00000260: 232a a906 2d03 8d8d 7497 02c4 00d8 c80d  #*..-...t.......
+00000270: 2dc3 26be 17f0 26f3 5dd5 390a ef7a e4fc  -.&...&.].9..z..
+00000280: e4cd c587 83b3 1ee9 9f93 d3b3 93df faaf  ................
+00000290: 7baf 49e9 e01c 9e4b 1af9 d0bf 7877 f2fe  {.I....K....xw..
+000002a0: 8240 89b3 83c1 c525 3979 430e 0697 e4d7  .@.....%9yC.....
+000002b0: fee0 b546 7abf 9f9e f5ce cfc9 c9d9 e646  ...Fz..........F
+000002c0: fff8 f4a8 df83 97fd c1e1 d1fb d7fd c15b  ...............[
+000002d0: f20a 2a0e 4e60 46f7 615e 03d4 8b13 822d  ..*.N`F.a^.....-
+000002e0: 4a58 fdde 3942 3bee 9d1d be83 c783 57fd  JX..9B;.......W.
+000002f0: a3fe c5a5 b6b9 f1a6 7f31 40a8 6f4e cec8  .........1@.oN..
+00000300: 0139 3d38 bbe8 1fbe 3f3a 3823 a7ef cf4e  .9=8....?:8#...N
+00000310: 4fce 7b80 c06b 803b e80f de9c 4133 bde3  O.{..k.;....A3..
+00000320: dee0 4287 66e1 1de9 fd06 0fe4 fcdd c1d1  ..B.f...........
+00000330: 11b6 b5b9 71f0 1e3a 7086 2892 c393 d3cb  ....q..:p.(.....
+00000340: b3fe db77 17e4 ddc9 d1eb 1ebc 7cd5 03dc  ...w........|...
+00000350: 0e5e 1df5 445b d0af c3a3 83fe b146 5e1f  .^..D[.......F^.
+00000360: 1c1f bced f15a 2700 06ba 87e5 0482 e4c3  .....Z'.........
+00000370: bb1e bec3 160f e0bf c38b fec9 007b 7278  .............{rx
+00000380: 32b8 3883 470d 3a7a 7691 d4fd d03f ef69  2.8.G.:zv....?.i
+00000390: e4e0 ac7f 8e34 7973 7672 0c7d 449a 4295  .....4ysvr.}D.B.
+000003a0: 130e 052a 0e7a 020c d29b 6486 058a e0f3  ...*.z....d.....
+000003b0: fbf3 5e02 91bc ee1d 1c01 b073 accc 7b19  ..^........s..{.
+000003c0: 9786 5155 4a54 d9ff 5f19 ff69 2ddb ff0d  ..QUJT.._..i-...
+000003d0: 65ff 3f89 fdbf 5b14 ff69 b4f6 1a0d c5d8  e.?...[..i......
+000003e0: 3fb2 fd7f faeb db6d d077 27df defe afb5  ?......m.w'.....
+000003f0: 1aed bcfd df82 7f94 fdff 14f6 3f0d 8db1  ............?...
+00000400: 111a dbbf 81e5 0966 db3e 69e8 f5cd 8d81  .......f.>i.....
+00000410: e1d0 7db2 3c39 3637 9272 7c9a 8021 1039  ..}.<967.r|..!.9
+00000420: 8e11 ccf7 c170 c242 044b 11ea 5e59 81e7  .....p.B.K..^Y..
+00000430: a2dd 0ee6 6840 4e7c ea1e f4c9 dbb9 c32d  ....h@N|.......-
+00000440: cdb7 31dc cd8d 779e 43b7 7d63 0aad cdc2  ..1...w.C.}c....
+00000450: d067 fbd5 ea14 6cf2 68a4 9b9e 53b5 d1f7  .g....l.h...S...
+00000460: 90ae 47f5 38c1 e120 02ab 3dd8 cfbb 26d2  ..G.8.. ..=...&.
+00000470: 8fd9 27ef 07bf 0e4e 3e0c c055 b18d 10da  ..'....N>..U....
+00000480: 7752 af64 a1ed 37e0 4900 04e1 e5a2 699a  wR.d..7.I.....i.
+00000490: 94f8 a12c 1a15 ff53 f1bf 24fe b7db 6eec  ...,...S..$...n.
+000004a0: 351b 2afe a7f4 7fbb 7ad6 3b78 7ddc d39d  5.*.....z.;x}...
+000004b0: f137 d7ff 3bed ce52 fcaf dd69 29fd ff14  .7..;..R...i)...
+000004c0: e967 9f18 b635 75bb 2550 8b21 0d4a bf6c  .g...5u.%P.!.J.l
+000004d0: 6e10 483f 5bce 94b0 c0ec 96ee aa96 ab23  n.H?[..........#
+000004e0: db1b 551d c372 ab6c e65d 9f06 1e06 a5f4  ..U..r.l.]......
+000004f0: a935 2991 6b6b 1cce baa5 76ad e6df 94aa  .5).kk....v.....
+00000500: d0c4 cf55 ff17 d4b4 2f08 567f 8b36 436f  ...U..../.V..6Co
+00000510: 6133 60ce 076a 4353 340e 6a15 1523 01f5  a3`..jCS4.j..#..
+00000520: 3d66 855e 307f 4e2e 307a 05ff 1984 598e  =f.^0.N.0z....Y.
+00000530: 6f53 32a7 21f1 bd6b 1a4c 223b 6390 8c29  oS2.!..k.L";c..)
+00000540: 830e d331 b74c 026a b9f0 af49 7996 4d8d  ...1.L.j...Iy.M.
+00000550: 4044 27a7 f0c8 7482 21b3 a967 d871 306b  @D'...t.!..g.q0k
+00000560: 0a76 11b6 0258 b9c6 9535 3542 0a2d 729b  .v...X...55B.-r.
+00000570: 070d 9b80 1ae6 0c5e 8418 fb04 709e c963  .......^....p..c
+00000580: 8a02 4e1a 070c 9c5a d399 3d27 264c 40cf  ..N....Z..='&L@.
+00000590: b1fe 3246 b608 c399 868b d1b6 8801 8618  ..2F............
+000005a0: 9e24 230f febc 896c 287c e8b9 2e10 1572  .$#....l(|.....r
+000005b0: 0634 bcf6 822f 8c94 df1c 0e2a bc22 645e  .4.../.....*."d^
+000005c0: 7976 840d 02c2 031a 05fc 9fb8 dce1 6050  yv............`P
+000005d0: e131 b817 2fc8 1b6a 8451 4019 3e6e 9397  .1../..j.Q@.>n..
+000005e0: 2f0f d348 7032 9f5b 7fd1 972f f7c9 a517  /..Hp2.[.../....
+000005f0: 718c 2808 0940 c018 ff01 4539 2918 9448  q.(..@....E9)..H
+00000600: c882 5580 2626 c60a a93b 05ea 7b51 20a8  ..U.&&...;..{Q .
+00000610: 283a 31b6 2613 1a08 1a5f 519b 4707 617c  (:1.&...._Q.G.a|
+00000620: 61a0 6eac 70ae 0b34 a02b a227 8301 f4c6  a.n.p..4.+.'....
+00000630: f181 7880 10a2 5140 bf64 1831 560a 5d24  ..x...Q@.d.1V.]$
+00000640: 8c1a 8e4d 1903 3453 744b 81f4 3ddb 322d  ...M..4StK..=.2-
+00000650: ca87 1500 38c6 170a 5326 e403 0804 21be  ....8...S&....!.
+00000660: 6dcc a781 1789 882c bdf1 6960 3905 3d08  m......,..i`9.=.
+00000670: e7be 88e4 ba82 c6ae a4b1 ecc5 bbc8 0182  ................
+00000680: 9d51 170c 2a72 ec8d 7907 3e18 21cc 8c14  .Q..*r..y.>.!...
+00000690: 55f8 54c3 502a 346d 6fa3 0a16 cd20 3967  U.T.P*4mo.... 9g
+000006a0: 1c42 2020 3800 4127 fd70 8b61 4496 70fa  .B  8.A'.p.aD.p.
+000006b0: 1b23 0c5a 6351 3772 4660 916b d00f 2860  .#.ZcQ7rF`.k..(`
+000006c0: d8cc 4b65 fe01 cdb9 74fe 5ce0 9532 c2ab  ..Ke....t.\..2..
+000006d0: 0b13 3c47 e884 cf44 1499 7138 2b6a 5a28  ..<G...D..q8+jZ(
+000006e0: 3026 8649 35a4 25b2 0d10 d34c c089 fe18  0&.I5.%....L....
+000006f0: c8fc 9404 06ce 0aa0 d90a 86b3 ad51 6004  .............Q`.
+00000700: 184e e6f1 7f7b ea05 50db 61f1 8ced bb20  .N...{..P.a.... 
+00000710: a76d 9bb3 130f 24f3 c87c 5634 a426 8886  .m....$..|V4.&..
+00000720: a4e6 13d7 1215 11b5 b115 00f3 c0f4 00c4  ................
+00000730: 3d31 16be 9052 000b 91f0 2d9f 07ca 3f7f  =1...R....-...?.
+00000740: fe3c 32d8 6c73 035e 2400 124d b9bd 7086  .<2.ls.^$..M..p.
+00000750: a0a0 c4ef 3d83 61c5 df7d 0703 e01c b1cf  ....=.a..}......
+00000760: 3166 20b3 3e13 d336 188b c1fb 73f0 60a0  1f .>..6....s.`.
+00000770: 2393 c073 0adc 2c62 0928 2900 4963 ef28  #..s..,b.().Ic.(
+00000780: 5f0a 5808 3a7a 63f0 7f81 b820 7749 b8a0  _.X.:zc.... wI..
+00000790: 4c9a 63e4 6020 3f70 3e98 7f0d 2abc 2c90  L.c.` ?p>...*.,.
+000007a0: 0546 7908 94a2 b6e5 52d6 8c8b 9e9e 9e20  .Fy.....R...... 
+000007b0: 6c68 9d74 d3f5 ca28 32ba edca e606 ce69  lh.t...(2......i
+000007c0: 1b32 a164 b974 6cfb a71c a392 8618 6be4  .2.d.tl.......k.
+000007d0: 8a06 238f 8149 1a97 d4f9 3429 871e 0cc4  ..#..I....4)....
+000007e0: 1059 8585 d467 dd3a 5a0b 9584 306f 409c  .Y...g.:Z...0o@.
+000007f0: 8fc1 9d05 c76e 0c24 80f1 e063 1744 a658  .....n.$...c.D.X
+00000800: 8fc0 8925 6905 fc02 7f01 7198 8ec0 d4b1  ...%i.....q.....
+00000810: 92f9 1867 7f2a df59 eb85 01a5 42eb d11b  ...g.*.Y....B...
+00000820: ca2b 57e4 4403 b584 6b23 e68c 9a5f 08b2  .+W.D...k#..._..
+00000830: 244e b88f 8750 7b44 065e 4847 9ef7 65d1  $N...P{D.^HG..e.
+00000840: 9089 ef75 90c9 d055 73a6 4f3d 6f6a 53de  ...u...Us.O=ojS.
+00000850: ae40 e156 a51b 375f 05a2 0e13 9aea 963f  .@.V..7_.......?
+00000860: 7747 42f0 7f7c fe11 3919 7889 702c eed2  wGB..|..9.x.p,..
+00000870: 38cc 591a 3251 607b 648c a754 6757 d3ca  8.Y.2Q`{d..TgW..
+00000880: 53e1 2db9 2bad f45f f321 6622 e705 39e0  S.-.+.._.!f"..9.
+00000890: a34b ce7d 9043 c922 9778 c7f0 1d57 1516  .K.}.C.".x...W..
+000008a0: 3303 1a4a 89d4 0206 608c 4b28 5190 e102  3..J....`.K(Q...
+000008b0: 5f00 5df0 71bd 0ce4 004c 8712 5f1e 8319  _.].q....L.._...
+000008c0: 598a 7cfc 6bd3 097f 1a7b d76e 498f 1b3f  Y.|.k....{.nI..?
+000008d0: 1931 1a5c 19cb 1878 a90c 8986 583d 63e4  .1.\...x....X=c.
+000008e0: 144d 1678 ffbb 96fc bcd4 c805 b718 7e8f  .M.x..........~.
+000008f0: 7f5c ea04 44c9 04a7 8d1f 8543 8b0d 7dcb  .\..D......C..}.
+00000900: 4495 8ddd 8111 e133 3688 707d b5b8 3594  D......36.p}..5.
+00000910: 0f8d d742 31f3 5ed7 c83e 0142 8773 8dd4  ...B1.^..>.B.s..
+00000920: 7149 7242 7cd9 ba46 1ab1 c112 bf8a fb77  qIrB|..F.......w
+00000930: 46af 8d60 cc12 ba4e 85d5 6552 eb0a 2535  F..`...N..eR..%5
+00000940: fcc4 7c94 3c60 da49 7b0a 2c20 4e43 282f  ..|.<`.I{., NC(/
+00000950: a172 894e 60e6 1976 3847 912b 9708 4175  .r.N`..v8G.+..Au
+00000960: 4ac6 c315 54c3 3513 6b4f 5644 80dc a242  J...T.5.kOVD...B
+00000970: 7e87 975f a89b 90be e75b 0c64 03b9 c005  ~.._.....[.d....
+00000980: 4b77 a117 50ec c9ac 5066 01aa d733 2a56  Kw..P...Pf...3*V
+00000990: 76e3 2e00 54ca 526d c57a e602 640b a02f  v...T.Rm.z..d../
+000009a0: 2c50 b0c3 6c0b cc15 2257 9585 7ce3 88a2  ,P..l..."W..|...
+000009b0: e123 8aa2 3561 a0f2 bd9e 81e1 01ca dbb8  .#..5a..........
+000009c0: 4aad 9582 948e ac30 29cf 6250 9ff1 e9f3  J......0).bP....
+000009d0: 4252 0014 8f04 91c8 e425 3521 dfe7 8934  BR.......%5!...4
+000009e0: 079e 7290 9428 b1b1 728c 32d8 7d72 f999  ..r..(..r.2.}r..
+000009f0: fc1f 398f 7cc4 51e2 0fa3 e3a0 3924 6d69  ..9.|.Q.....9$mi
+00000a00: 332e c9e5 2117 e231 e0c8 4533 8cc0 9443  3...!..1..E3...C
+00000a10: c5c9 fb80 ca73 4c0d 3e0a f8db 8191 bb12  .....sL.>.......
+00000a20: 6a1b de4c b89d 6490 5134 d5c8 d873 b742  j..L..d.Q4...s.B
+00000a30: 0214 c545 743e 8a1e 0a1a acc5 5844 e512  ...Et>......XD..
+00000a40: b1c3 6d2d 1f2c 5918 803f 23e8 838e f665  ..m-.,Y..?#....e
+00000a50: 0034 8149 8e73 96db 6168 66fa 3ed0 856f  .4.I.s..ahf.>..o
+00000a60: 0010 2be4 695d cd4d b731 0e4e 0823 4c46  ..+.i].M.1.N.#LF
+00000a70: 73a9 ca0d 9854 a6e5 f3a9 f09c ab62 d199  s....T.......b..
+00000a80: 8915 2f6e 2ffc 0524 2af8 0589 1a98 5a38  ../n/..$*.....Z8
+00000a90: 6888 1eba 83cf 2565 531b 23b8 c598 c240  h.....%eS.#....@
+00000aa0: 2ef2 83a2 e146 1ab7 4316 5b29 7472 4ec5  .....F..C.[)trN.
+00000ab0: a07d 9611 c6cf 7ceb 02a7 a5d0 514c 57f1  .}....|.....QLW.
+00000ac0: 3fb5 fffb 9f8f ff15 edff eeb4 5abb 2d15  ?...........Z.-.
+00000ad0: 04fc a1e3 7fcb 19d5 afe1 fffb edff dea9  ................
+00000ae0: 77da 6aff b75a ff51 e3ff 84eb 3f20 ffeb  w.j..Z.Q....? ..
+00000af0: 2df8 a3d6 7f94 fc2f 94ff a950 8eee cf1f  -....../...P....
+00000b00: 6bfd 0758 bd93 93ff 8d5a a7d1 56eb 3f4f  k..X.....Z..V.?O
+00000b10: 9164 c86e bad8 9191 8d03 c631 3d1e 5660  .d.n.......1=.V`
+00000b20: 9b1b f2d1 9fe3 4a48 f2e8 18e1 2c79 7023  ......JH....,yp#
+00000b30: c707 178e 11d7 47cf 6973 8347 3e33 81c0  ......G.is.G>3..
+00000b40: 04bc 0e4f 957d b1e4 e4c8 ad28 a44b fe2e  ...O.}.....(.K..
+00000b50: 89e0 f710 c37f acb4 4f3e 9678 4c1c 2330  ........O>.xL.#0
+00000b60: c174 3434 82c0 9897 3ee1 9328 37f1 b154  .t44....>..(7..T
+00000b70: bdf1 5f6c 0f81 8de9 840c 87d0 6438 1c96  .._l........d8..
+00000b80: 31dc a191 14c8 eec0 7371 b336 8f47 6acb  1.......sq.6.Gj.
+00000b90: 5196 ee1b c366 3cac 7d33 c4d8 832c ef5b  Q....f<.}3...,.[
+00000ba0: 37d4 1ee2 cb2b c38e 68b7 d16e c7c8 632a  7....+..h..n..c*
+00000bb0: 954a 8b87 3e34 6d19 362e 92ac 0a52 eb31  .J..>4m.6....R.1
+00000bc0: b298 f6c1 7f35 9c34 9262 d5c3 e191 0c2f  .....5.4.b...../
+00000bd0: 5e0d c887 752d 8c88 e460 60b7 44e5 f41a  ^...u-...``.D...
+00000be0: 0dfb 33c2 4de4 c8c9 cb55 9628 b04f 3ecc  ..3.M....U.(.O>.
+00000bf0: 2854 132d 8a6c c266 5e64 8f71 750a dc78  (T.-.l.f^d.qu..x
+00000c00: 514e 5fd1 7d24 b9ce 9bef 722c 7239 d7e0  QN_.}$....r,r9..
+00000c10: 937b d743 59a0 5d6f e4f2 97e3 5edd 651c  .{.CY.]o....^.e.
+00000c20: 7375 e2c1 82a2 f1cf 5c89 dcf8 41c1 dc9b  su......\...A...
+00000c30: f480 5893 55a8 6040 6209 5497 c06c 484d  ..X.U.`@b.T..lHM
+00000c40: 8645 5716 c1b9 a108 ce75 2537 e9af bc9b  .EW......u%7....
+00000c50: b2ed 5d77 6b1a 5f0d c4f9 a4e1 7e7b 9f76  ..]wk._.....~{.v
+00000c60: cb09 0135 92fa 59af 6864 8ceb 4f5d d7d7  ...5..Y.hd..O]..
+00000c70: 23cb 0d77 2b8b 26a9 bd12 e71c 627e 0055  #..w+.&.....b~.U
+00000c80: cb5b b94e 6c69 b917 95af eb4e 0e5a d2b5  .[.Nli.....N.Z..
+00000c90: ba56 d4b9 f53d 63f4 01b4 ad09 1627 dba4  .V...=c......'..
+00000ca0: 9e34 ded2 9286 a091 4a7a c439 4811 12ce  .4......Jz.9H...
+00000cb0: 437b 2d23 c8e5 560a abc5 2f8c 9207 619a  C{-#..V.../...a.
+00000cc0: 7931 4684 4283 f098 68ea b52b 27ab 1476  y1F.B...h..+'..v
+00000cd0: 1fb3 92ee d312 ccfc 44fb a5db 289c 803f  ........D...(..?
+00000ce0: f309 98eb 4cba e56e 1a8f a56e 0b86 8442  ....L..n...n...B
+00000cf0: 8874 2ecf b43d f34b 9295 92af 531a 0e61  .t...=.K....S..a
+00000d00: 08f8 5c5d 2908 df52 b11a 6646 015f 3d4d  ..\])..R..fF._=M
+00000d10: 07ab a568 5a29 1381 e451 e00a 5956 507f  ...hZ)...Q..YVP.
+00000d20: 95f0 59cf bac5 a2a0 887f 79f4 bc0b 7a4c  ..Y.......y...zL
+00000d30: ff8b 061e 2b3f 8429 6338 1f79 8561 2afa  ....+?.)c8.y.a*.
+00000d40: 9f7d 71a9 91da 2768 acde 6813 f282 1cf0  .}q...'h..h.....
+00000d50: 3875 1c8f 1721 fc29 283d 627a b617 ac04  8u...!.)(=bz....
+00000d60: 9f2c 23a4 1f63 d0d0 4104 7d91 8df5 0bd8  .,#..c..A.}.....
+00000d70: d733 8c52 1700 1743 40c4 7ae7 fd25 cd12  .3.R...C@.z..%..
+00000d80: 09ef cffc 4917 6bda 6d34 c45e 160d 6fb5  ....I.k.m4.^..o.
+00000d90: da78 1051 e316 8bc9 baaa b547 23f2 92d0  .x.Q.......G#...
+00000da0: 93e5 8048 dc02 2adf 6152 aded 4005 17ee  ...H..*.aR..@...
+00000db0: 502e 96b7 eb95 25d6 8e57 65d6 f3f7 a161  P.....%..We....a
+00000dc0: 9b91 cdc3 fec0 a5bd c8b4 71d5 c05d ace9  ..........q..]..
+00000dd0: 8c68 784d e5f2 4bcc c409 5dc4 8767 9955  .hxM..K...]..g.U
+00000de0: 9842 ee7f 20b4 428c 2515 d168 d5d9 9f41  .B.. .B.%..h...A
+00000df0: 28f9 3a26 12a8 8b1c 592b e4e5 4bd2 203f  (.:&....Y+..K. ?
+00000e00: 914c c1cb a582 97a2 e032 2571 cbc3 fda4  .L.......2%q....
+00000e10: 24df 24e1 0829 b9d8 d071 aba0 3c00 4271  $.$..)...q..<.Bq
+00000e20: 0566 0473 bedc 23bf b64c 832e 5e6c bb85  .f.s..#..L..^l..
+00000e30: 587f 6727 6229 0602 56b7 a041 66c2 a4b8  X.g'b)..V..Af...
+00000e40: 376b 9133 2815 c028 79ce 10fe 0e93 3d35  7k.3(..(y.....=5
+00000e50: c378 08f9 6b81 d17a 829d e3c2 2211 b072  .x..k..z...."..r
+00000e60: 1380 d7c6 bd04 2c0a 64e7 c11f 09e8 620b  ......,.d.....b.
+00000e70: cf5a ab75 31ee 317f bbbe 445a c72d 2f53  .Z.u1.1...DZ.-/S
+00000e80: 1a30 6e5a a4e4 183a 12f5 b45d f1b1 f669  .0nZ...:...]...i
+00000e90: 15d8 cbc7 051b cfda 6f00 f4ab 315d 8005  ........o...1]..
+00000ea0: d167 5309 1c94 c518 4c89 72a5 c8a4 bbdf  .gS.....L.r.....
+00000eb0: 14c9 b25a 0c78 bdbc e2fb 31ac 49b1 04b1  ...Z.x....1.I...
+00000ec0: c4a2 30c3 7d7e 06bb 5d34 0520 eeef 0d4b  ..0.}~..]4. ...K
+00000ed0: 23dc bf24 1e3a 58d7 16a3 b730 5f79 695e  #..$.:X....0_yi^
+00000ee0: 7673 839f d835 e959 962d 7499 a115 6ed8  vs...5.Y.-t...n.
+00000ef0: 08a5 63cc 281d 4b0f d7f3 f9da 307f 5a49  ..c.(.K.....0.ZI
+00000f00: c133 cae8 2df2 483a a200 5888 6fc9 a7f8  .3..-.H:..X.o...
+00000f10: 426e 502a f041 45db 20c4 c6e2 ab65 dc76  BnP*.AE. ....e.v
+00000f20: e9cb b56a 6e46 43b3 612c cdb2 4d17 ea0c  ...jnFC.a,..M...
+00000f30: 4bb8 e019 8b13 0995 92ad 2b05 41e4 d3a0  K.........+.A...
+00000f40: ccd5 2327 1310 08ff 2cbb 0b0f 9cae 98d2  ..#'....,.......
+00000f50: 6875 5352 142d ea94 0045 6c33 f95c 9954  huSR.-...El3.\.T
+00000f60: 7278 88bd 517c 5f14 14ae 1539 b219 67a0  rx..Q|_....9..g.
+00000f70: 4b64 44a5 9007 e3a8 0a0c 0bcd 222d 6764  KdD........."-gd
+00000f80: 0a77 8d63 989e 5b88 859c 5ac2 9b5a 3993  .w.c..[...Z..Z9.
+00000f90: 7a37 d4c4 7d0b e828 f12d 90dc 7f47 5b49  z7..}..(.-...G[I
+00000fa0: 6e93 b865 8209 f062 b4e5 a61f 546a c617  n..e...b....Tj..
+00000fb0: ba6a 4eb8 f43a 8bbc d8c2 a225 9b45 f81e  .jN..:.....%.E..
+00000fc0: 9ad0 0823 a6dd 75b2 c896 bbf2 870e 469e  ...#..u.......F.
+00000fd0: 53ae 20dd 2dc6 770f a24a 34e4 d903 60bb  S. .-.w..J4...`.
+00000fe0: b963 6ebd 55b8 8527 2be5 062c 0609 4359  .cn.U..'+..,..CY
+00000ff0: 3840 6915 0568 2f09 889f b8c7 9bc4 60c0  8@i..h/.......`.
+00001000: 01ce c709 162d d4d7 b670 59d8 c2e5 bd5a  .....-...pY....Z
+00001010: 68dc de07 e366 a90f dc6b afad 86da bc1d  h....f...k......
+00001020: ef25 a897 4550 97cd 6c03 6432 4c4e 9372  .%..EP..l.d2LN.r
+00001030: f153 deea bb60 d8e3 1e6f def8 5686 2392  .S...`...o..V.#.
+00001040: 5d46 e384 4b13 0597 e51c be57 aa4b c0d6  ]F..K......W.K..
+00001050: 262f 0bad 263e 6770 936f 0a26 9f23 ed5a  &/..&>gp.o.&.#.Z
+00001060: ed31 25c7 3792 0d61 10b9 a624 0457 704b  .1%.7..a...$.WpK
+00001070: d232 2da5 7e82 9997 46a4 9c0d e23d 17f1  .2-.~...F....=..
+00001080: 8685 664b d7fd a59b 0df9 e52d 8934 26a8  ..fK.......-.4&.
+00001090: a245 ee7a 2996 1704 b8f5 2881 b32c e404  .E.z).....(..,..
+000010a0: 19d6 9b1a 67c5 315b 6977 6344 496e 682b  ....g.1[iwcDInh+
+000010b0: 1455 a205 fc4e 21e0 5f1d 4cf8 6ef1 38fa  .U...N!._.L.n.8.
+000010c0: cd03 c39a 8c31 dd66 47ac 1ae6 452c bdd8  .....1.fG...E,..
+000010d0: d15c 37e2 dce2 ca64 dd85 1686 eccd 7d22  .\7....d......}"
+000010e0: 3f8f 4808 d121 a18d 87f1 e719 223e 91f1  ?.H..!......">..
+000010f0: a857 f9cb 7948 7c3b e13a 406b 6215 858c  .W..yH|;.:@kb...
+00001100: 28e3 7071 f430 99fd 7762 50b1 2aa3 a3dd  (.pq.0..wbP.*...
+00001110: 53ae 1466 81ac c1af 1c0a 8b64 e380 b90a  S..f.......d....
+00001120: 68e6 60e3 e56c 1d4c e57c 445f 5b8a f157  h.`..l.L.|D_[..W
+00001130: 2acb 3d15 51c5 8775 3413 9694 98a2 fda0  *.=.Q..u4.......
+00001140: 1fe2 bbac 5432 0d10 de6c 51ee 3ce2 df2c  ....T2...lQ.<..,
+00001150: 94ef 89b6 00a3 4f2c db2e 97eb 8d5d 8dc4  ......O,.....]..
+00001160: 7f2a 99e6 7c63 ccf7 1077 9717 3a5e e237  .*..|c...w..:^.7
+00001170: d3a9 102d 867b e225 90a5 c2db a401 1524  ...-.{.%.......$
+00001180: b414 780b 241e 5fc9 896b 2ea0 5417 fa38  ..x.$._..k..T..8
+00001190: 8391 1cc9 c0b8 d671 b769 6e08 45c7 b4ec  .......q.in.E...
+000011a0: 4b74 eff0 bf8a 5638 8dce 96c1 a4fa ae2d  Kt....V8.......-
+000011b0: 7e24 c8a5 7e66 eba5 5ba8 3c06 da7c 11e5  ~$..~f..[.<..|..
+000011c0: 6188 8351 93a7 efcb 6291 01de adf6 1860  a..Q....b......`
+000011d0: ea85 60b2 95b5 a517 0fa0 a069 05a6 4def  ..`........i..M.
+000011e0: 4443 41c0 021a 9617 fd2b 178a bf9f 6082  DCA......+....`.
+000011f0: b72b 386d b308 2f0d 468e 3a55 d25c d507  .+8m../.F.:U.\..
+00001200: 74fc 6eb8 bcc7 0f88 1601 78b4 3f2b c5e2  t.n.......x.?+..
+00001210: 8ff7 17bf 4829 18e8 c21e 8b5e e3d4 e1ff  ....H).....^....
+00001220: 578a b2f3 53bb 708c 6f0a ab16 b0f6 c3a1  W...S.p.o.......
+00001230: 892f 29eb f929 f0e4 8428 c638 e9d0 43aa  ./)..)...(.8..C.
+00001240: aea6 d3bd 08f1 35c6 ad68 5d1f d9a0 1d25  ......5..h]....%
+00001250: 8562 c18f 6ccb c550 a598 d8f4 0a6d 183f  .b..l..P.....m.?
+00001260: 72fc 5b54 6fe4 8fc1 a2cc eaa8 ac4e 0355  r.[To........N.U
+00001270: 064a ac78 9910 373a 7caa dc71 9120 04a6  .J.x..7:|..q. ..
+00001280: 61be c78a 2640 62a8 48f4 18aa 457c 2156  a...&@b.H...E|!V
+00001290: 3358 732c 2950 a980 237c 4319 aedb a258  3Xs,)P..#|C....X
+000012a0: 6854 5690 1c0d 42c0 9fdd 167f c322 6b42  hTV...B......"kB
+000012b0: 3885 86eb c22c 42f7 082d 86fd b544 fe33  8....,B..-...D.3
+000012c0: 5a69 0289 2cb5 f34b edff 54fb bf96 ceff  Zi..,..K..T.....
+000012d0: dd6d eda8 fd9f 6aff 67f1 fecf 783f ddbd  .m....j.g...x?..
+000012e0: 367f 3ebb fdfc af5a ab95 dfff d9ac a9f3  6.>....Z........
+000012f0: 3f9e 24f1 dd9e 7a6a 6f66 c1f7 de8a 4b94  ?.$...zjof....K.
+00001300: feff a6fa 5f9d fff9 cfe9 ffa2 f33f 3b7b  ...._........?;{
+00001310: addd e6ae b202 94fe 4f67 e874 3add c665  ........Og.t:..e
+00001320: 90ea 03f8 ff7e dfff 7576 763a eafb 3fe5  .....~..uvv:..?.
+00001330: ffa9 f17f 42ff 2f91 ffca ff53 f27f adfc  ....B./....S....
+00001340: bfe7 d9d0 f73e ffb9 51eb eca8 efff 9e24  .....>..Q......$
+00001350: dded fce7 6d75 feb3 d2ff 4aff 2bfd af92  ....mu....J.+...
+00001360: d2ff 5ef5 fce4 fdd9 61ef 5c0f 6fc2 c7d0  ..^.....a.\.o...
+00001370: ffed 9d7c fcb7 dede 51f7 3f3c 4992 0a70  ...|....Q.?<I..p
+00001380: 2339 ee7b 83d1 30f2 757f be71 eb09 101b  #9.{..0.u..q....
+00001390: ebd7 0836 ee62 426e dc71 9ead 2d37 a63e  ...6.bBn.q..-7.>
+000013a0: ae8e bbe6 7c68 5bee 1776 6b05 3c7e ce0a  ....|h[..vk.<~..
+000013b0: e8ed 0543 cf1f f203 8b79 493c 76af 8a7f  ...C.....yI<v...
+000013c0: 86d4 6073 5e7c c8b7 3599 ae3b a482 262b  ..`s^|..5..;..&+
+000013d0: cbf8 be27 cb28 fdaf f4bf d2ff 2afd cfea  ...'.(......*...
+000013e0: ff22 79fb 15fa bf56 abe7 f47f b3d3 54fe  ."y....V......T.
+000013f0: ff93 24c5 ea3f 7652 fa5f e97f a5ff 95fe  ..$..?vR._......
+00001400: bf97 fe4f bb4f 8fe0 ffd7 5af9 f3ff 1a8d  ...O.O....Z.....
+00001410: 9dba d2ff 4f91 c4a6 e86e b7a1 d7f5 e6c2  ....O....n......
+00001420: 15ee 766b 7a63 57af 2b49 a0f4 bfd2 ff4a  ..vkzcW.+I.....J
+00001430: ffab a4f4 ff8a a8e8 23e8 ff46 33af ff5b  ........#..F3..[
+00001440: 75b5 fffb 1f1a 7fc5 fc4a ff3f b1fe 57f7  u........J.?..W.
+00001450: bffc 73fa bfe8 fe97 dd66 6bb7 ade4 c00f  ..s......fk.....
+00001460: adff c532 b039 993e 0eff afd5 ffed 468e  ...2.9.>......F.
+00001470: ff5b f586 5aff 7f92 f411 8c3a 7e2e d4a7  .[..Z......:~...
+00001480: cd8d d098 0e47 9165 e3a9 49e2 09bf 548f  .....G.e..I...T.
+00001490: 8f93 53bc a2f4 bff2 ffbf 77ff 7fa7 b3a3  ..S.......w.....
+000014a0: fc7f a5ff 63fd ff28 9b95 6ed3 ff3b 3bf5  ....c..(..n..;;.
+000014b0: bcfe afd5 3b4a ff3f 4512 3779 e358 879e  ....;J.?E.7y.X..
+000014c0: 67b3 e4ba 1f7c a3f1 ab53 87be 617e 31a6  g....|...S..a~1.
+000014d0: 9489 cb7c 788e 3c4f c6c5 a583 ade5 29b4  ...|x.<O......).
+000014e0: 254f e5b9 12df 0a74 b7f8 948a df8e 2933  %O.....t......)3
+000014f0: 038b 9fac d9dd 7ac8 5703 3120 837f 06d0  ......z.W.1 ....
+00001500: ddca 7c06 1067 4681 dddd baeb 2705 5b5a  ..|..gF.....'.[Z
+00001510: 7c3a e40b 0975 481d c302 0878 b5ac ce7f  |:...uH....x....
+00001520: ff47 5e0e 8e50 e246 62d2 7433 842a c7e7  .G^..P.Fb.t3.*..
+00001530: 15c9 abe3 87f1 7a59 f7e3 e244 9aad ccca  ......zY...D....
+00001540: cb56 ea1c a3ad a555 9838 176c b4c7 3eb8  .V.....U.8.l..>.
+00001550: 467d ffad beff 5ef6 ffeb adbd 6647 5901  F}....^.....fGY.
+00001560: 3fb2 fee7 fb98 1f8f ffef f7fd 7793 afff  ?...........w...
+00001570: abef bf95 ffa7 c6ff 69fd bf56 5bf9 7f4a  ........i..V[..J
+00001580: fec7 f27f fdb7 2e8f e4ff b56a 9d46 fefb  ...........j.F..
+00001590: afa6 fafe fb69 52ec efcd 59f1 fdad c97d  .....iR...Y....}
+000015a0: af38 15e4 e5b0 40b1 914d 8723 8351 3c5d  .8....@..M.#.Q<]
+000015b0: 9635 63af f1f4 f484 bb88 73a6 fb78 b996  .5c.......s..x..
+000015c0: e1e3 7702 e52d 5daf e29d 09d9 9b65 17fb  ..w..-]......e..
+000015d0: 0ad6 9f3e 26eb e1b4 7369 78ed 055f e242  ...>&...six.._.B
+000015e0: be67 5be6 7cf8 e5da 08a6 d23b c533 48f9  .g[.|......;.3H.
+000015f0: a4c5 2b18 a838 cadf 8247 bc52 04bf c04a  ..+..8...G.R...J
+00001600: ee1c 4a4e 19bd 80d2 f10d 3e78 42ac 8d87  ..JN......>xB...
+00001610: 8ca6 aa5a a6b8 bb0d faa6 e7aa bec8 5ff2  ...Z.........._.
+00001620: 9a76 60e3 abc8 384c 511e b249 3773 0fee  .v`...8LQ..I7s..
+00001630: ea0b 68f1 d602 6de9 be59 79a2 a9c0 b38b  ..h...m..Yy.....
+00001640: 3895 4b87 ae7b ca09 51c2 2baf aeb4 2c59  8.K..{..Q.+...,Y
+00001650: ba99 270d 5df2 91c7 68b7 26af fda9 25c7  ..'.]...h.&...%.
+00001660: b7be 2017 8121 af5d 4921 cd7f ea36 3502  .. ..!.]I!...65.
+00001670: b72c ae60 4075 c1af 61e8 3680 5bd3 f591  .,.`@u..a.6.[...
+00001680: 94b9 eade 081a 1d02 ae28 3252 b7e9 c437  .........(2R...7
+00001690: 70c4 37d6 7c94 5750 a1df 6f2d ce7b ae63  p.7.|.WP..o-.{.c
+000016a0: 0bfb f9ab 5600 225e d142 b1a2 c0cf 0f28  ....V."^.B.....(
+000016b0: 5e7c 5686 e62a 997b 32e2 7b1d e007 5ec9  ^|V..*.{2.{...^.
+000016c0: c196 ee74 90a8 f13b 6be4 6d35 99e3 6717  ...t...;k.m5..g.
+000016d0: 5749 0066 1c44 fee0 60ec 413c d5ad dc99  WI.f.D..`.A<....
+000016e0: b305 dd4f 112c 7315 9518 d409 4eba 1915  ...O.,s.....N...
+000016f0: b745 4df9 7507 2eb1 29c3 1786 4bda 9260  .EM.u...)...K..`
+00001700: 7893 110c a531 95a7 a9cb cb42 5d5f 6791  x....1.....B]_g.
+00001710: 53e6 652a fce6 954e bda3 9149 e922 3dbb  S.e*...N...I."=.
+00001720: f108 ddcc 0c87 b910 39fb e4ef 4cf5 ff96  ........9...L...
+00001730: 9659 0ab9 cf72 a7f7 6527 59ed bb66 a4c6  .Y...r..e'Y..f..
+00001740: d732 d243 39a9 91e2 a461 e80d 036a 9833  .2.C9....a...j.3
+00001750: 79d0 7c8a b178 3688 f611 0dc4 8ade 1db8  y.|..x6.........
+00001760: 2d5d 277b 5dcb bf94 0ff3 fd8f d932 d591  -]'{]........2..
+00001770: 4a41 ad3c 59be 15f7 366a b7b2 af43 0db7  JA.<Y...6j...C..
+00001780: 5cd4 950a bfe1 b796 65e6 9921 b899 cf2a  \.......e..!...*
+00001790: 71b5 1a1e 7f9d 34af 9373 d3c3 cbbc ff5e  q.....4..s.....^
+000017a0: 0b3a 6675 0bef 4cc7 a0ee 70c8 0f4a 1f02  .:fu..L...p..J..
+000017b0: cb58 ee70 189f 952e ac00 1d5f aa13 b495  .X.p......._....
+000017c0: ffaf fcff efca ffdf dddb 6bef ec28 ff5f  ..........k..(._
+000017d0: f9ff 6bfd fffb 9f63 718b ffdf 6cb5 f2e7  ..k....cq...l...
+000017e0: bfd5 5b75 b5ff eb5f ebff 3fd4 857f 68dc  ..[u..._..?...h.
+000017f0: e05e 8efd 9d7c 0968 f00e fe44 b3c8 9fe0  .^...|.h...D....
+00001800: 171b 16b9 0fc7 b69f 751f 1ed5 d5ae af73  ........u......s
+00001810: 10b6 d211 0be7 fe8e f7bf c9f5 fe27 9def  .............'..
+00001820: 7ce4 67bd 6fdd aaef ed81 73bd d6b7 be8f  |.g.o.....s.....
+00001830: 0ffd 8833 b7fd 2f9a b9eb 7d5b 98ba 3e0d  ...3../...}[..>.
+00001840: f815 bbae 49ef 3e75 efe3 e9fe 6ff8 badf  ....I.>u....o...
+00001850: 9db7 bbfb 95ce eeee 837c 5de5 eaaa a492  .........|].....
+00001860: 4a2a a9a4 924a 2aa9 a492 4a2a a9a4 924a  J*...J*...J*...J
+00001870: 2aa9 a492 4a2a a9a4 924a 2aa9 a492 4a2a  *...J*...J*...J*
+00001880: a9a4 924a 2aa9 a492 4a2a a9a4 924a df79  ...J*...J*...J.y
+00001890: fa7f 8a4f 5c2e 00f0 0000                 ...O\.....
```

