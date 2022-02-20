# openzo
> Opensea 클론 코딩

[Homepage](https://openzo.vercel.app/)      
[GitHub](https://github.com/codestates/BEB_02_openzo)

### Home
![front](/image/front.png)

### List
![list](/image/list.png)

### Create
![create](/image/create.png)


# Stack
> NodeJs, MongoDB

# 맡은 역할
> Backend
+ NFT 리스트 DB 저장
+ Transfer시 DB 업데이트

## Schema
# NFT 모델
|Key|Type|Detail|
|---|---|---|
|tokenId|String|tokenId|
|creator|String|nft 발행자|
|description|Array|NFT 특징|
|image|String|NFT 이미지 주소|
|name|String|NFT 이름|
|ownerAddr|String|NFT 소유자|

## API (/nft)
+ / (get)
    + Nft 전체 리스트 조회
+ /token/{tokenId} (get)
    + tokenId로 NFT detail 조회
+ /addr/{addr} (get)
    + 가지고있는 nft 주소로 검색
+ /savenft (post)
    + NFT 정보 저장
+ /transfer (post)
    + nft transfer시 Db 업데이트

# Keep
+ 팀원들과 지속적인 소통을 통해 프로젝트가 원할하게 진행 되었다

# Problem
+ Github 사용시 flow를 잘 설정


# Try
+ Infura websocket을 활용하여 블록체인 데이터를 가져와 DB 동기화
+ Https 설정