# PC기반 제어 시스템이란?

---
대강 봤을 때는 시스템 프로그래밍이랑 비슷한 맥락의 개념인 것 같다. 같이 등장하는 키워드를 보면 #시스템 프로그래밍 #자동화 #PLC #스마트팩토리 등등. 한번 알아보자!

- 시스템 소프트웨어: 어플리케이션 sw가 hw 및 저수준 기능을 사용할 수 있도록 도와주는 소프트웨어. 운영체제가 제공하는 서비스를 직접 이용한다.

말 그대로 기계를 제어하기 위해 pc를 사용하는 것이다. 기존의 plc가 하던 일을 pc가 대신하게 되는 것.

pc -(output 디지털/아날로그 출력)-> 머신

pc <-(input 디지털/아날로그 입력)- 머신

OS는 주로 Windows, Linux 사용. 윈도우는 hard real time을 구현하지 못함. 그래서 RTOS(real time os)를 별도로 설치해서 사용함.

또 Control SW에 개발/실행환경을 사용함.

이런 여러가지 부분들을 모두 사용해서 일종의 plc의 역할을 하도록 만듬.

pc기반제어 SW들... visual studio(C, C++, C#), labVIEW, matlab/simulink, TwinCAT 등.

결론 : 공장기기 등을 제어하기 위한 시스템인 것 같다!

임베디드 컨트롤러, HW와의 인터페이스, HW와의 통신, HW&SW의 통합 등

관련 공고:
[(주)아이브 공고](https://www.saramin.co.kr/zf_user/jobs/relay/view?isMypage=no&rec_idx=46550237&recommend_ids=eJxNzssNwzAMg%2BFpeqcepqhzB8n%2BW9RJALnHD7R%2FKEsrl%2FKS2ae%2BGZ0Fx9Xwm6Uw%2BaxVMiI28RIswybfx9mGIXbL9JdiwDisUK6cvwRJm7KYQZ91EXjW9wz2rmiY3mHrHJlU9KE5w4eC2HXIdp4U3aLjMGPHb%2F4AWhVASw%3D%3D&view_type=search&searchword=%EB%A9%80%ED%8B%B0%EC%8A%A4%EB%A0%88%EB%93%9C&searchType=search&gz=1&t_ref_content=generic&t_ref=search&relayNonce=4091dc98aa4f1d111c3c&paid_fl=n&search_uuid=d965789c-311b-4cd7-a9b1-80447bc70fe3&immediately_apply_layer_open=n#seq=0)
