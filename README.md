# Wechat Portal 

列出与 SeeDAO 有关的微信群组, 说明群组目的, 加入方式等

## 新增/修改/删除微信群组

请修改本目录下的 `index.html` ，移动到 `allGroups` 区块:

```js
// ...
allGroups: [
    { id: 1001, name: 'SeeDAO 市政厅校友群', type: 'contributor', permission: '需审核', info: '由担任过市政厅岗位，了解市政厅运行运作的 SeeDAO 贡献者组成', condtion: '需曾任市政厅岗位', contactMethod: '微信联系 Ricky : .....' },
    // ...

    { id: 2001, name: 'SeeDAO 深圳据点', type: 'local', permission: '开放加入', info: '深圳地方 SeeDAO 小伙伴交流群', condtion: '', contactMethod: '微信联系 Ricky : .....' },
    // ...

    { id: 3001, name: 'SeeDAO 治理公会', type: 'project', permission: '开放加入', info: '前身为 SeeDAO 运营公会, 后改为治理公会, 自由交流讨论社区治理事项', condtion: '', contactMethod: '微信联系 Ricky : ....' },
    // ...
],
// ...
```
可以发现目前有三个区块, 根据你的微信群归类到三个区块底下, 以 JSON 格式填写:
1. `id` 请递增, `type` 根据区块选择 `contributor` `local` `project`
2. `permission` 请选择 `开放加入`, `邀请制`, `需审核` 三种其中一种
3. 将群组名称写到 `name`, 群组基本信息写在 `info`, 联络方式写在 `contactMethod` 三者没有格式限制, 不要太长为佳
