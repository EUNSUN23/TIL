###Promise.all 사용해서 await 병합하기

```js
const getDeptAPI = async () => {
  const deptRes = await axios.get("http://localhost:3008/api/dept");
  return deptRes.data.packet;
};

const getTitleAPI = async () => {
  const titleRes = await axios.get("http://localhost:3008/api/title");
  return titleRes.data.packet;
};

export const getEmployeeAPI = async () => {
  return Promise.all([getDeptAPI, getTitleAPI]).then((res) => {
    return { dept: res[0], title: res[1] };
  });
};
```

- getTitleAPI, getDeptAPI 두가지 통신을 한번에 처리한다.
