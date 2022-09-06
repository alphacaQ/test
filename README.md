실행방법:
  - 윈도우 GUI : Aimaps_T-toolw.exe 실행
  - 콘솔실행 : Aimaps_T-toolc.exe 실행

콘솔 실행환경 options:
  - -h, --help					show this help message and exit
  - --tif <path>				/path/from/tif_folder/
                        			* tif파일 경로(폴더)
						* ex) D:\data\tif
  - --shp <path> (optional)			/path/from/shpfilename/	
    						* shp파일 경로(.shp 파일명)
						* ex) D:\data\annotation.shp
  - --save <path>				/path/to/save/folder/	
						* 저장할 폴더경로
						* ex) D:\data\tile
  - --save-filename <filename>		* 저장할 파일명(이미지와 json에 적용됨), 확장자 제외
						* NIA 노지작물 데이터 구축용 네이밍 규칙 : 날짜 6자리 + 지역코드 3자리
						* ex) 220906KW1
  - --index <number> (optional)		* 1, 10 등 저장될 파일명의 인덱스 시작번호(MAX : 9999), 기본값 : 0
						* ex) 10 입력시 저장될 파일명 : 220906KW10010
  - --size <pixel size>			* 512, 800, 1024 등 타일링 이미지의 픽셀 사이즈(정수형)
  - --boundary <image or shp>		* image 또는 shp 입력
		                        	* image : 이미지 경계로 타일링, shp : 어노테이션 경계로 타일링
  - --save-rate <number> (optional)	* 타일링 이미지에서 어노테이션 폴리곤이 차지하는 비율(0~100), 기본값 : 0
						* ex) 20 입력시 저장될 타일 이미지에서 어노테이션이 차지하는 비율이 20이상이면 타일 생성됨
  - --crops <code>				* code : C, R (C : 배추, R : 무)