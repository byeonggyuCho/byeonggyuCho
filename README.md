    안녕하세요 프론트엔드 개발자 조병규입니다.
    사용자에게 직관적인 서비스, 동료에게 가독성이 좋은 코드를 제공하는 것을 중요하게 생각합니다.
    웹을 통해 사회의 편리함을 제공하는 일에 관심이 있습니다.
    유연한 근무환경과 오픈 커뮤니케이션을 지향하며
    React와 Typescript 그리고 작업물을 문서화하는 것을 좋아합니다.

- 이름: 조병규
- 나이: 31살 (1991년생)
- 학력: 대졸 (한국교통대학교, 기계공학)
- 병역: 육군 만기제대(11.09 ~ 13.06)
- 거주지: 서울 동작구
- e-mail: byeonggyu303@gmail.com
- Skill
  - front: React(+Redux), Typescript, ES6+, Scss
  - back: Node.js, Mysql, MongoDB
  - etc: Git, Jenkins, Webpack, Babel


```ts
type Education = {
  university: string;
  major: string;
};

interface Info {
  name: string;
  age: number;
  education?: Education;
  skill?: string[];
  experience?: [];
  phone?: string;
  email?: string;
  address?: string;
}

type RequiredInfo = Required<Pick<Info, 'name' | 'age'>>;

class Profile implements Info {
  public name: string;
  public age: number;
  public education?: Education;
  public phone?: string;
  public email?: string;
  public address?: string;
  public skill?: string[];

  constructor(info: RequiredInfo) {
    this.name = info.name;
    this.age = info.age;
  }
}

const profile = new Profile({ name: '조병규', age: 31 });

profile.phone = '01089265827';
profile.email = 'byeonggyu303@gmail.com';
profile.address = '서울시 동작구';
profile.education = {
  university: '한국교통대학교',
  major: '기계공학과',
};
profile.skill = [
  'react',
  'typescript',
  'nodeJs',
  'ES6+',
  'Scss',
  'StyledComponent',
  'webpack',
];



```
