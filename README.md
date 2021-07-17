# kotlinSpringBoot
최근 Java 단점을 보완하여 나온 Kotlin을 많이 사용하는 추세로, 공부할겸 kotlin/SpringBoot로 WebService를 만들어본다.   

## Project Focus
### Kotlin의 특징 및 장점
> Kotlin <-> Java의 호환가능.   
> ..
### REST 지향
> 1. StateLess. (Server가 상태를 저장하지 않음.)
> 2. Cache. (Clinet는 응답을 재사용할 수 있어야함.)
> 3. Layerd System.(Server, Client 사이에 Firewall, Proxy 등 다계층 형태를 구성/확장 가능해야한다.   
> 4. Interface의 일관성. (Architect의 단순화 -> 독립성 유지.)
>> 4.1 Resource 식별.
>> 4.2 Msg를 통한 Resouce Control.
>> 4.3 Self Descriptive .
>> 4.4 HATEOAS.
> 5. Code On Demand.(Server에서 특정 Code를 전달하여 Client에서 실행.)

### Ultimate goal
> 1. Use Kotlin.
> 2. Use jpa.
> 3. Use Spring Security.
> 4. Asynchronize. (Webflux)
> 5. Deploy using Docker.
> 6. MicroService.
> 7. Monitoring.

## MEMO
1. URI, URL : Identifer, Location의 차이. '식별자'이므로 Internet에서 특정 Resource를 나타내는 Address이며,Unique하다. Location은 위치에 해당하므로, URL은 URI의 하위개념이다.
2. URL 설계원칙 (RFC-3986)
> 2.1 '/'는 계층관계를 나타낸다. 마지막 문자로 '/'를 사용하지 않는다.
> 2.2 '-'는 가독성을 위해 사용하며, '_'는 사용하지 않는다.
> 2.3 소문자를 주로 사용하며, 확장자나 언어에 관련된 문자, Code 내 의존적인 Path를 사용하지 않는다. 
> 2.4 Session ID를 포함하지 않는다.
> 2.5 Method명을 사용하지않는다. (CRUD 포함.)
