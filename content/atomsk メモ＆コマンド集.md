[Atomsk](https://atomsk.univ-lille.fr/)
1. コマンドプロンプトを起動
mkdir test_atomsk　 ←test_atomskなるフォルダを現在ログインしているユーザーのフォルダに作成 
cd test_atomsk　←test_atomskなるフォルダを作業ディレクトリに指定(読み込むファイルや出力ファイルはファイルパスを指定しない限りここに集約される)

以下使用したことのあるコマンド
- atomsk 8YSZ.cif -duplicate 10 10 10 -dislocation 0.5*box 0.5*box screw Z Y 2.58 8YSZ_screw.cif
- atomsk 8YSZ.cif -rotate x 90 -rotate  z 45 -duplicate 10 10 10 -disloc 0.5*box 0.5*box screw y x 3.64867099923 8YSZ_screw.cif
- atomsk 8YSZ.cif -rotate x 90  -duplicate 10 10 10 -disloc 0.5*box 0.5*box screw y x 3.64867099923 8YSZ_screw.cif
- atomsk 8YSZ.cif -duplicate 10 10 10 -dislocation 0.5*box 0.5*box edge_rm Z Y 3.64867099923 0.3 8YSZ_edge.cif
- atomsk 8YSZ.cif -duplicate 10 10 10 -dislocation 0.5*box 0.5*box edge_add Z Y 3.64867099923 0.3 8YSZ_edgeadd.cif
- atomsk 8YSZ.cif -duplicate 10 10 10 -dislocation 0.5*box 0.5*box edge_add Z Y 2.56 0.3 8YSZ_edgeadd.cif
- atomsk 8YSZ.cif -duplicate 10 10 10 -crack I stress 20 30.0 0.5*BOX z y 90 0.3 8YSZ_crack.cif
- atomsk 8YSZ.cif -duplicate 10 10 10 -crack I stress 40 30 0.5*BOX z y 90 0.3 -crack II stress 10 30 0.5*BOX z y 90 0.3 -crack III stress 10 30 0.5*BOX z y 90 0.3 8YSZ_fract.cif
- atomsk 8YSZ.cif -duplicate 10 10 10 -disloc loop 0.501*BOX 0.501*BOX 0.501*BOX Z 10 3.634528 0 0 0.33 8YSZ_loop.cif
- atomsk YSZ_unrelaxed.cif -disloc loop 0.501*BOX 0.501*BOX 0.501*BOX Z 10 3.634528 0 0 0.33 YSZ_unrelaxed_loop.cif
- atomsk YSZ_unrelaxed.cif -disloc 0.5*box 0.5*box screw y x 3.64867099923 YSZ_unrelaxed_screw.cif
- atomsk YSZ_unrelaxed.cif -disloc 0.5*box 0.5*box screw y x 3.64867099923 YSZ_unrelaxed_screw.cif
- atomsk YSZ_unrelaxed.cif -disloc loop 0.333*BOX 0.333*BOX 0.333*BOX Z 10 3.634528 0 0 0.33 YSZ_unrelaxed_loop.cif
- atomsk YSZ_unrelaxed.cif -disloc 0.333*box 0.333*box screw y x 3.64867099923 YSZ_unrelaxed_screw.cif
- atomsk YSZ_2unrelaxed.cif -duplicate 5 5 5 -disloc 0.5*box 0.5*box screw y x 3.64867099923 YSZ_unrelaxed_screw.cif
- atomsk Diamond.cif -duplicate 3 3 3 -disloc 0.5*box 0.5*box screw y x 2.52233 Diamond_screw.cif
- atomsk Diamond.cif -duplicate 5 5 5 -disloc 0.5*box 0.5*box edge_add y x 2.52233 Diamond_edgeadd.cif
- atomsk Diamond.cif -duplicate 5 5 5 -disloc 0.5*box 0.5*box edge_rm y x 2.52233 Diamond_edgerm.cif
- atomsk Diamond.cif -duplicate 3 3 3 -disloc loop 0.5*box 0.5*box 0.5*box z 3 3.56712 0 0 0.3 Diamond_loop.cif
- atomsk Diamond.cif -duplicate 3 3 3 Diamond_extended.cif
- atomsk Diamond.cif -duplicate 3 3 3 -rotate  z 45 -rotate z 54.7  -disloc 0.5*box 0.5*box screw y x 2.52233 Diamond_screw2.cif

