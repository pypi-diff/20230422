# Comparing `tmp/voyager_cpu-0.2.2.tar.gz` & `tmp/voyager_cpu-0.2.3.tar.gz`

## Comparing `voyager_cpu-0.2.2.tar` & `voyager_cpu-0.2.3.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/.gitmodules
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/src/voyagercpu/__init__.py
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/src/voyagercpu/cpu.py
--rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/src/voyagercpu/decoder.py
--rwxr-xr-x   0        0        0     1658 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/src/voyagercpu/example.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/src/voyagercpu/ram.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/src/voyagercpu/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/test_decoder.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/test_utils.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/.git
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/LICENSE.md
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/README.md
--rwxr-xr-x   0        0        0     9992 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-add
--rw-r--r--   0        0        0    20574 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-add.dump
--rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-addi
--rw-r--r--   0        0        0    13070 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-addi.dump
--rwxr-xr-x   0        0        0     9728 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-and
--rw-r--r--   0        0        0    21504 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-and.dump
--rwxr-xr-x   0        0        0     9416 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-andi
--rw-r--r--   0        0        0    11014 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-andi.dump
--rwxr-xr-x   0        0        0     9160 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-auipc
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-auipc.dump
--rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-beq
--rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-beq.dump
--rwxr-xr-x   0        0        0     9656 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bge
--rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bge.dump
--rwxr-xr-x   0        0        0     9656 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bgeu
--rw-r--r--   0        0        0    15926 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bgeu.dump
--rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-blt
--rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-blt.dump
--rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bltu
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bltu.dump
--rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bne
--rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bne.dump
--rwxr-xr-x   0        0        0    13296 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-fence_i
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-fence_i.dump
--rwxr-xr-x   0        0        0     9212 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jal
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jal.dump
--rwxr-xr-x   0        0        0     9356 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jalr
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jalr.dump
--rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lb
--rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lb.dump
--rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lbu
--rw-r--r--   0        0        0    13852 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lbu.dump
--rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lh
--rw-r--r--   0        0        0    14974 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lh.dump
--rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lhu
--rw-r--r--   0        0        0    14881 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lhu.dump
--rwxr-xr-x   0        0        0     9228 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lui
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lui.dump
--rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lw
--rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lw.dump
--rwxr-xr-x   0        0        0     9728 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-or
--rw-r--r--   0        0        0    21498 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-or.dump
--rwxr-xr-x   0        0        0     9416 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-ori
--rw-r--r--   0        0        0    12304 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-ori.dump
--rwxr-xr-x   0        0        0    13976 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sb
--rw-r--r--   0        0        0    20302 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sb.dump
--rwxr-xr-x   0        0        0    13992 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sh
--rw-r--r--   0        0        0    22900 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sh.dump
--rwxr-xr-x   0        0        0     9072 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-simple
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-simple.dump
--rwxr-xr-x   0        0        0    10088 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sll
--rw-r--r--   0        0        0    21039 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sll.dump
--rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slli
--rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slli.dump
--rwxr-xr-x   0        0        0     9992 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slt
--rw-r--r--   0        0        0    19209 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slt.dump
--rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slti
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slti.dump
--rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltiu
--rw-r--r--   0        0        0    13035 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltiu.dump
--rwxr-xr-x   0        0        0     9992 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltu
--rw-r--r--   0        0        0    19249 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltu.dump
--rwxr-xr-x   0        0        0    10112 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sra
--rw-r--r--   0        0        0    23533 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sra.dump
--rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srai
--rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srai.dump
--rwxr-xr-x   0        0        0    10112 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srl
--rw-r--r--   0        0        0    22212 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srl.dump
--rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srli
--rw-r--r--   0        0        0    14428 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srli.dump
--rwxr-xr-x   0        0        0     9968 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sub
--rw-r--r--   0        0        0    19453 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sub.dump
--rwxr-xr-x   0        0        0    14008 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sw
--rw-r--r--   0        0        0    23150 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sw.dump
--rwxr-xr-x   0        0        0     9728 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xor
--rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xor.dump
--rwxr-xr-x   0        0        0     9416 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xori
--rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xori.dump
--rwxr-xr-x   0        0        0    19320 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-add
--rw-r--r--   0        0        0    50940 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-add.dump
--rwxr-xr-x   0        0        0    18408 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-addi
--rw-r--r--   0        0        0    44295 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-addi.dump
--rwxr-xr-x   0        0        0    19016 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-and
--rw-r--r--   0        0        0    52483 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-and.dump
--rwxr-xr-x   0        0        0    17944 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-andi
--rw-r--r--   0        0        0    42045 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-andi.dump
--rwxr-xr-x   0        0        0    17312 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-auipc
--rw-r--r--   0        0        0    37344 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-auipc.dump
--rwxr-xr-x   0        0        0    18368 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-beq
--rw-r--r--   0        0        0    44877 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-beq.dump
--rwxr-xr-x   0        0        0    18536 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bge
--rw-r--r--   0        0        0    46181 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bge.dump
--rwxr-xr-x   0        0        0    18588 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bgeu
--rw-r--r--   0        0        0    47442 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bgeu.dump
--rwxr-xr-x   0        0        0    18368 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-blt
--rw-r--r--   0        0        0    44880 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-blt.dump
--rwxr-xr-x   0        0        0    18420 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bltu
--rw-r--r--   0        0        0    46172 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bltu.dump
--rwxr-xr-x   0        0        0    18372 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bne
--rw-r--r--   0        0        0    44918 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bne.dump
--rwxr-xr-x   0        0        0    18340 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-fence_i
--rw-r--r--   0        0        0    40966 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-fence_i.dump
--rwxr-xr-x   0        0        0    17376 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jal
--rw-r--r--   0        0        0    37323 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jal.dump
--rwxr-xr-x   0        0        0    17680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jalr
--rw-r--r--   0        0        0    39400 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jalr.dump
--rwxr-xr-x   0        0        0    18792 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lb
--rw-r--r--   0        0        0    44158 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lb.dump
--rwxr-xr-x   0        0        0    18792 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lbu
--rw-r--r--   0        0        0    44181 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lbu.dump
--rwxr-xr-x   0        0        0    18796 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lh
--rw-r--r--   0        0        0    45143 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lh.dump
--rwxr-xr-x   0        0        0    18796 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lhu
--rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lhu.dump
--rwxr-xr-x   0        0        0    17404 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lui
--rw-r--r--   0        0        0    37466 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lui.dump
--rwxr-xr-x   0        0        0    18804 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lw
--rw-r--r--   0        0        0    46280 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lw.dump
--rwxr-xr-x   0        0        0    19028 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-or
--rw-r--r--   0        0        0    52871 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-or.dump
--rwxr-xr-x   0        0        0    17972 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-ori
--rw-r--r--   0        0        0    42597 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-ori.dump
--rwxr-xr-x   0        0        0    23124 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sb
--rw-r--r--   0        0        0    51034 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sb.dump
--rwxr-xr-x   0        0        0    23132 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sh
--rw-r--r--   0        0        0    53687 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sh.dump
--rwxr-xr-x   0        0        0    17136 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-simple
--rw-r--r--   0        0        0    36157 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-simple.dump
--rwxr-xr-x   0        0        0    19528 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sll
--rw-r--r--   0        0        0    52370 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sll.dump
--rwxr-xr-x   0        0        0    18404 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slli
--rw-r--r--   0        0        0    44152 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slli.dump
--rwxr-xr-x   0        0        0    19296 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slt
--rw-r--r--   0        0        0    50379 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slt.dump
--rwxr-xr-x   0        0        0    18388 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slti
--rw-r--r--   0        0        0    43758 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slti.dump
--rwxr-xr-x   0        0        0    18388 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltiu
--rw-r--r--   0        0        0    43778 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltiu.dump
--rwxr-xr-x   0        0        0    19296 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltu
--rw-r--r--   0        0        0    50420 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltu.dump
--rwxr-xr-x   0        0        0    19628 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sra
--rw-r--r--   0        0        0    53977 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sra.dump
--rwxr-xr-x   0        0        0    18456 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srai
--rw-r--r--   0        0        0    45348 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srai.dump
--rwxr-xr-x   0        0        0    19604 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srl
--rw-r--r--   0        0        0    53292 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srl.dump
--rwxr-xr-x   0        0        0    18432 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srli
--rw-r--r--   0        0        0    44760 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srli.dump
--rwxr-xr-x   0        0        0    19264 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sub
--rw-r--r--   0        0        0    50482 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sub.dump
--rwxr-xr-x   0        0        0    23152 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sw
--rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sw.dump
--rwxr-xr-x   0        0        0    19024 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xor
--rw-r--r--   0        0        0    52793 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xor.dump
--rwxr-xr-x   0        0        0    17980 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xori
--rw-r--r--   0        0        0    42762 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xori.dump
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/README.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 voyager_cpu-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/.gitmodules
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/src/voyagercpu/__init__.py
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/src/voyagercpu/cpu.py
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/src/voyagercpu/decoder.py
+-rwxr-xr-x   0        0        0     1667 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/src/voyagercpu/example.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/src/voyagercpu/ram.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/src/voyagercpu/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/test_decoder.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/.git
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/LICENSE.md
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/README.md
+-rwxr-xr-x   0        0        0     9992 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-add
+-rw-r--r--   0        0        0    20574 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-add.dump
+-rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-addi
+-rw-r--r--   0        0        0    13070 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-addi.dump
+-rwxr-xr-x   0        0        0     9728 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-and
+-rw-r--r--   0        0        0    21504 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-and.dump
+-rwxr-xr-x   0        0        0     9416 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-andi
+-rw-r--r--   0        0        0    11014 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-andi.dump
+-rwxr-xr-x   0        0        0     9160 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-auipc
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-auipc.dump
+-rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-beq
+-rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-beq.dump
+-rwxr-xr-x   0        0        0     9656 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bge
+-rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bge.dump
+-rwxr-xr-x   0        0        0     9656 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bgeu
+-rw-r--r--   0        0        0    15926 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bgeu.dump
+-rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-blt
+-rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-blt.dump
+-rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bltu
+-rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bltu.dump
+-rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bne
+-rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bne.dump
+-rwxr-xr-x   0        0        0    13296 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-fence_i
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-fence_i.dump
+-rwxr-xr-x   0        0        0     9212 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jal
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jal.dump
+-rwxr-xr-x   0        0        0     9356 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jalr
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jalr.dump
+-rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lb
+-rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lb.dump
+-rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lbu
+-rw-r--r--   0        0        0    13852 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lbu.dump
+-rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lh
+-rw-r--r--   0        0        0    14974 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lh.dump
+-rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lhu
+-rw-r--r--   0        0        0    14881 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lhu.dump
+-rwxr-xr-x   0        0        0     9228 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lui
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lui.dump
+-rwxr-xr-x   0        0        0    13748 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lw
+-rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lw.dump
+-rwxr-xr-x   0        0        0     9728 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-or
+-rw-r--r--   0        0        0    21498 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-or.dump
+-rwxr-xr-x   0        0        0     9416 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-ori
+-rw-r--r--   0        0        0    12304 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-ori.dump
+-rwxr-xr-x   0        0        0    13976 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sb
+-rw-r--r--   0        0        0    20302 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sb.dump
+-rwxr-xr-x   0        0        0    13992 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sh
+-rw-r--r--   0        0        0    22900 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sh.dump
+-rwxr-xr-x   0        0        0     9072 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-simple
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-simple.dump
+-rwxr-xr-x   0        0        0    10088 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sll
+-rw-r--r--   0        0        0    21039 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sll.dump
+-rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slli
+-rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slli.dump
+-rwxr-xr-x   0        0        0     9992 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slt
+-rw-r--r--   0        0        0    19209 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slt.dump
+-rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slti
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slti.dump
+-rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltiu
+-rw-r--r--   0        0        0    13035 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltiu.dump
+-rwxr-xr-x   0        0        0     9992 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltu
+-rw-r--r--   0        0        0    19249 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltu.dump
+-rwxr-xr-x   0        0        0    10112 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sra
+-rw-r--r--   0        0        0    23533 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sra.dump
+-rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srai
+-rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srai.dump
+-rwxr-xr-x   0        0        0    10112 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srl
+-rw-r--r--   0        0        0    22212 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srl.dump
+-rwxr-xr-x   0        0        0     9680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srli
+-rw-r--r--   0        0        0    14428 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srli.dump
+-rwxr-xr-x   0        0        0     9968 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sub
+-rw-r--r--   0        0        0    19453 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sub.dump
+-rwxr-xr-x   0        0        0    14008 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sw
+-rw-r--r--   0        0        0    23150 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sw.dump
+-rwxr-xr-x   0        0        0     9728 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xor
+-rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xor.dump
+-rwxr-xr-x   0        0        0     9416 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xori
+-rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xori.dump
+-rwxr-xr-x   0        0        0    19320 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-add
+-rw-r--r--   0        0        0    50940 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-add.dump
+-rwxr-xr-x   0        0        0    18408 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-addi
+-rw-r--r--   0        0        0    44295 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-addi.dump
+-rwxr-xr-x   0        0        0    19016 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-and
+-rw-r--r--   0        0        0    52483 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-and.dump
+-rwxr-xr-x   0        0        0    17944 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-andi
+-rw-r--r--   0        0        0    42045 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-andi.dump
+-rwxr-xr-x   0        0        0    17312 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-auipc
+-rw-r--r--   0        0        0    37344 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-auipc.dump
+-rwxr-xr-x   0        0        0    18368 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-beq
+-rw-r--r--   0        0        0    44877 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-beq.dump
+-rwxr-xr-x   0        0        0    18536 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bge
+-rw-r--r--   0        0        0    46181 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bge.dump
+-rwxr-xr-x   0        0        0    18588 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bgeu
+-rw-r--r--   0        0        0    47442 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bgeu.dump
+-rwxr-xr-x   0        0        0    18368 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-blt
+-rw-r--r--   0        0        0    44880 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-blt.dump
+-rwxr-xr-x   0        0        0    18420 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bltu
+-rw-r--r--   0        0        0    46172 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bltu.dump
+-rwxr-xr-x   0        0        0    18372 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bne
+-rw-r--r--   0        0        0    44918 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bne.dump
+-rwxr-xr-x   0        0        0    18340 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-fence_i
+-rw-r--r--   0        0        0    40966 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-fence_i.dump
+-rwxr-xr-x   0        0        0    17376 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jal
+-rw-r--r--   0        0        0    37323 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jal.dump
+-rwxr-xr-x   0        0        0    17680 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jalr
+-rw-r--r--   0        0        0    39400 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jalr.dump
+-rwxr-xr-x   0        0        0    18792 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lb
+-rw-r--r--   0        0        0    44158 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lb.dump
+-rwxr-xr-x   0        0        0    18792 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lbu
+-rw-r--r--   0        0        0    44181 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lbu.dump
+-rwxr-xr-x   0        0        0    18796 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lh
+-rw-r--r--   0        0        0    45143 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lh.dump
+-rwxr-xr-x   0        0        0    18796 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lhu
+-rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lhu.dump
+-rwxr-xr-x   0        0        0    17404 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lui
+-rw-r--r--   0        0        0    37466 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lui.dump
+-rwxr-xr-x   0        0        0    18804 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lw
+-rw-r--r--   0        0        0    46280 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lw.dump
+-rwxr-xr-x   0        0        0    19028 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-or
+-rw-r--r--   0        0        0    52871 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-or.dump
+-rwxr-xr-x   0        0        0    17972 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-ori
+-rw-r--r--   0        0        0    42597 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-ori.dump
+-rwxr-xr-x   0        0        0    23124 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sb
+-rw-r--r--   0        0        0    51034 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sb.dump
+-rwxr-xr-x   0        0        0    23132 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sh
+-rw-r--r--   0        0        0    53687 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sh.dump
+-rwxr-xr-x   0        0        0    17136 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-simple
+-rw-r--r--   0        0        0    36157 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-simple.dump
+-rwxr-xr-x   0        0        0    19528 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sll
+-rw-r--r--   0        0        0    52370 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sll.dump
+-rwxr-xr-x   0        0        0    18404 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slli
+-rw-r--r--   0        0        0    44152 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slli.dump
+-rwxr-xr-x   0        0        0    19296 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slt
+-rw-r--r--   0        0        0    50379 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slt.dump
+-rwxr-xr-x   0        0        0    18388 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slti
+-rw-r--r--   0        0        0    43758 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slti.dump
+-rwxr-xr-x   0        0        0    18388 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltiu
+-rw-r--r--   0        0        0    43778 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltiu.dump
+-rwxr-xr-x   0        0        0    19296 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltu
+-rw-r--r--   0        0        0    50420 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltu.dump
+-rwxr-xr-x   0        0        0    19628 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sra
+-rw-r--r--   0        0        0    53977 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sra.dump
+-rwxr-xr-x   0        0        0    18456 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srai
+-rw-r--r--   0        0        0    45348 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srai.dump
+-rwxr-xr-x   0        0        0    19604 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srl
+-rw-r--r--   0        0        0    53292 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srl.dump
+-rwxr-xr-x   0        0        0    18432 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srli
+-rw-r--r--   0        0        0    44760 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srli.dump
+-rwxr-xr-x   0        0        0    19264 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sub
+-rw-r--r--   0        0        0    50482 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sub.dump
+-rwxr-xr-x   0        0        0    23152 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sw
+-rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sw.dump
+-rwxr-xr-x   0        0        0    19024 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xor
+-rw-r--r--   0        0        0    52793 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xor.dump
+-rwxr-xr-x   0        0        0    17980 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xori
+-rw-r--r--   0        0        0    42762 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xori.dump
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/LICENSE.md
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/README.md
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 voyager_cpu-0.2.3/PKG-INFO
```

### Comparing `voyager_cpu-0.2.2/src/voyagercpu/cpu.py` & `voyager_cpu-0.2.3/src/voyagercpu/cpu.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 INST_ALIGN = 4
 PC_REG_INDEX = 32
 
 class AlignmentError(Exception):
     pass
 
 class VoyagerCPU:
-    def __init__(self, start_pc=0):
+    def __init__(self, start_pc=0, verbose=0):
         self.regfile = self.reset_regs()
         self.regfile[PC_REG_INDEX] = start_pc
         self.time_period = 0
+        self.verbose = verbose
 
     def __str__(self) -> str:
         dump_str = f"Time period: {self.time_period}\n"
         dump_str += "Register states:\n"
         for i, r in enumerate(self.regfile.keys()):
             dump_str += f"{REG_DICT[i]}: {self.regfile[r]} \t"
             if (i + 1) % 5 == 0:
@@ -38,14 +39,16 @@
 
     def __decode(self, raw_inst: int) -> RVInst:
         decoded_inst = decode_instruction(raw_inst)
         logger.debug(f"Decoded: {decoded_inst}")
         return decoded_inst
 
     def __execute(self, inst: RVInst):
+        if self.verbose:
+            print(inst)
         mne = inst.mnemonic
         r = self.regfile # For brevity
 
         if type(inst) == UType:
             if mne == Instruction.LUI:
                 r[inst.rd] = inst.imm
             elif mne == Instruction.AUIPC:
@@ -128,23 +131,22 @@
                 r[inst.rd] = res
             elif mne == Instruction.SRA:
                 r[inst.rd] = r[inst.rs1] >> r[inst.rs2]
             elif mne == Instruction.OR:
                 r[inst.rd] = r[inst.rs1] | r[inst.rs2]
             elif mne == Instruction.AND:
                 r[inst.rd] = r[inst.rs1] & r[inst.rs2]
-        else:
-            logger.debug("System instructions not implemented")
+        elif verbose:
+            print("Instruction not implemented")
 
     def next_cycle(self, ram):
         raw_inst = self.__fetch(ram)
         decoded_inst = self.__decode(raw_inst)
         self.__execute(decoded_inst)
 
         # Confirm that the PC is aligned at a multiple of 4
         if self.regfile[PC_REG_INDEX] & 0b11:
             raise AlignmentError(f"Program counter is misaligned! - " \
                                  f"PC: {self.regfile[PC_REG_INDEX]}")
         
         self.regfile[PC_REG_INDEX] += INST_ALIGN
-        logger.debug(self.__str__())
         self.time_period += 1
```

### Comparing `voyager_cpu-0.2.2/src/voyagercpu/decoder.py` & `voyager_cpu-0.2.3/src/voyagercpu/decoder.py`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/src/voyagercpu/example.py` & `voyager_cpu-0.2.3/src/voyagercpu/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 PROGRAM_PROMPT = "> Select test program - (1, default) rv32ui-p-xor, " \
     "(2) rv32ui-p-add, " \
     "(3) rv32ui-p-srai: "
 SEG_N = 1
 TEST_PROGRAM_PATH =  "./tests/riscv-tests-prebuilt-binaries/isa/rv32ui/"
 
 if __name__ == "__main__":
-    voyager_cpu = VoyagerCPU()
+    voyager_cpu = VoyagerCPU(verbose=1)
     voyager_ram = VoyagerRAM()
 
     usr_in = input(PROGRAM_PROMPT)
     f = TEST_PROGRAM_PATH
     
     if "2" in usr_in:
         f += "rv32ui-p-add"
```

### Comparing `voyager_cpu-0.2.2/src/voyagercpu/ram.py` & `voyager_cpu-0.2.3/src/voyagercpu/ram.py`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/src/voyagercpu/utils.py` & `voyager_cpu-0.2.3/src/voyagercpu/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logging.basicConfig()
+logger = logging.getLogger("voyagercpu")
+logger.setLevel(logging.ERROR)
 
 def abi_register_names() -> list:
     """
     Returns a list of RISC-V ABI register names.
 
     Returns:
         list: List of ABI register names as strings.
@@ -17,15 +18,15 @@
         [f"s{i}" for i in range(2, 12)] + \
         [f"t{i}" for i in range(3, 7)] + ["pc"]
 
 def register_names() -> list:
     """
     Returns a list of basic RISC-V register names.
 
-    These have the form x0-31. Their ABI names 
+    These have the form x0-31. Their ABI names
     may be derived using `abi_register_names()`.
 
     Returns:
        list: List of register names as strings.
     """
     return [f"x{i}" for i in range(32)] + ["pc"]
```

### Comparing `voyager_cpu-0.2.2/tests/test_decoder.py` & `voyager_cpu-0.2.3/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/test_utils.py` & `voyager_cpu-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/LICENSE.md` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-add` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-add`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-add.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-add.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-addi` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-addi`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-addi.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-addi.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-and` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-and`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-and.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-and.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-andi` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-andi`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-andi.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-andi.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-auipc` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-auipc`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-auipc.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-auipc.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-beq` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-beq`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-beq.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-beq.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bge` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bge`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bge.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bge.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bgeu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bgeu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bgeu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bgeu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-blt` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-blt`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-blt.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-blt.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bltu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bltu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bltu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bltu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bne` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bne`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bne.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-bne.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-fence_i` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-fence_i`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-fence_i.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-fence_i.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jal` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jal`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jal.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jal.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jalr` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jalr`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jalr.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-jalr.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lb` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lb`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lb.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lb.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lbu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lbu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lbu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lbu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lh` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lh`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lh.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lh.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lhu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lhu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lhu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lhu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lui` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lui`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lui.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lui.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lw` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lw`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lw.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-lw.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-or` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-or`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-or.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-or.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-ori` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-ori`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-ori.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-ori.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sb` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sb`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sb.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sb.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sh` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sh`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sh.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sh.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-simple` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-simple`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-simple.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-simple.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sll` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sll`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sll.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sll.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slli` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slli`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slli.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slli.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slt` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slt`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slt.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slt.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slti` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slti`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slti.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-slti.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltiu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltiu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltiu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltiu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sltu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sra` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sra`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sra.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sra.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srai` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srai`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srai.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srai.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srl` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srl`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srl.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srl.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srli` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srli`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srli.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-srli.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sub` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sub`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sub.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sub.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sw` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sw`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sw.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-sw.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xor` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xor`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xor.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xor.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xori` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xori`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xori.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-p-xori.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-add` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-add`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-add.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-add.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-addi` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-addi`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-addi.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-addi.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-and` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-and`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-and.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-and.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-andi` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-andi`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-andi.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-andi.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-auipc` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-auipc`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-auipc.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-auipc.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-beq` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-beq`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-beq.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-beq.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bge` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bge`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bge.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bge.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bgeu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bgeu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bgeu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bgeu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-blt` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-blt`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-blt.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-blt.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bltu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bltu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bltu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bltu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bne` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bne`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bne.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-bne.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-fence_i` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-fence_i`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-fence_i.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-fence_i.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jal` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jal`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jal.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jal.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jalr` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jalr`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jalr.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-jalr.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lb` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lb`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lb.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lb.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lbu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lbu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lbu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lbu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lh` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lh`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lh.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lh.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lhu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lhu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lhu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lhu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lui` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lui`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lui.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lui.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lw` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lw`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lw.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-lw.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-or` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-or`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-or.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-or.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-ori` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-ori`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-ori.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-ori.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sb` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sb`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sb.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sb.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sh` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sh`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sh.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sh.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-simple` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-simple`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-simple.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-simple.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sll` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sll`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sll.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sll.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slli` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slli`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slli.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slli.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slt` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slt`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slt.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slt.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slti` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slti`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slti.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-slti.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltiu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltiu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltiu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltiu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltu` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltu`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltu.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sltu.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sra` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sra`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sra.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sra.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srai` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srai`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srai.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srai.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srl` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srl`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srl.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srl.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srli` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srli`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srli.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-srli.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sub` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sub`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sub.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sub.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sw` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sw`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sw.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-sw.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xor` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xor`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xor.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xor.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xori` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xori`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xori.dump` & `voyager_cpu-0.2.3/tests/riscv-tests-prebuilt-binaries/isa/rv32ui/rv32ui-v-xori.dump`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/LICENSE.md` & `voyager_cpu-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/README.md` & `voyager_cpu-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `voyager_cpu-0.2.2/pyproject.toml` & `voyager_cpu-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "voyager-cpu"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Carlton Shepherd", email="carlton@linux.com" },
 ]
 description = "A simple 32-bit RISC-V CPU emulator"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
```

### Comparing `voyager_cpu-0.2.2/PKG-INFO` & `voyager_cpu-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voyager-cpu
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple 32-bit RISC-V CPU emulator
 Project-URL: Homepage, https://github.com/cgshep/voyager-cpu
 Project-URL: Bug Tracker, https://github.com/cgshep/voyager-cpu/issues
 Author-email: Carlton Shepherd <carlton@linux.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 2 - Pre-Alpha
```

