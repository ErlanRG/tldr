# lz4

> .lz4 파일을 압축하거나 압축 해제합니다.
> 더 많은 정보: <https://github.com/lz4/lz4>.

- 파일 압축:

`lz4 {{경로/대상/파일}}`

- 파일 압축 해제:

`lz4 -d {{파일.lz4}}`

- 파일 압축 해제 후 `stdout`에 출력:

`lz4 -dc {{파일.lz4}}`

- 디렉토리 및 그 내용 패키징 및 압축:

`tar cvf - {{경로/대상/폴더}} | lz4 - {{디렉토리.tar.lz4}}`

- 디렉토리 및 그 내용 압축 해제 및 풀기:

`lz4 -dc {{디렉토리.tar.lz4}} | tar -xv`

- 최고 압축률로 파일 압축:

`lz4 -9 {{경로/대상/파일}}`
