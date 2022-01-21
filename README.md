# locale-zh-Hans

这个代码仓库包含了 State of JS/CSS/etc 的中文语言文件。你可以在此处查看所有支持的 [语言仓库列表](https://github.com/StateOfJS/?q=locale-&type=&language=&sort=) 。

## 如何贡献代码

#### 1. 成为翻译者

要开始帮助我们翻译调查，你应该 [加入 Discord](https://discord.com/invite/zRDb35jfrt) 并向我发送你的 GitHub 用户名以及区域设置代码用于你想帮助的语言。

然后，我们会授予你对包含所有翻译 `yml` 文件的 repo 的维护者权限，从现在开始，你可以与翻译团队的其他成员一起管理它。

#### 2. 寻找要翻译的东西

你可以通过浏览调查结果网站等方式查找未翻译的字符串，或者使用我们的 API 获取额外的数据，比如说：

```graphql
query GetLocaleData {
  locale(localeId: "ru-RU") {
    completion
    totalCount
    translatedCount
    translators
    untranslatedKeys
  }
}
```

#### 3. 记录你的名字

每位翻译人员都会呈现在网站的贡献列表中。虽然这最终将通过 GitHub API 自动完成，但现在你可以在此处添加你的姓名：

- https://github.com/StateOfJS/Monorepo/blob/main/api/src/data/locales.yml

#### 4. 实时推送你的更改

目前没有通过 GitHub Hooks 来更新翻译好的语言文件，所以目前最好的方法是在 Discord 发私信给管理员，通知他更新网站。

## 翻译文件说明

#### 调查相关文件

这些文件中的翻译会在调查问卷中出现。

- `surveys.yml`
- `accounts.yml`
- `state_of_js_2020_survey.yml`

#### 调查结果相关文件

这些文件中的翻译会在调查结果中出现。

- `results.yml`
- `state_of_css_2020.yml`
- `state_of_js_2020.yml`

#### 公用文件

这些文件中的翻译既会在调查问卷中出现，也会在调查结果中出现。

- `common.yml`
- `state_of_css.yml`
- `state_of_js.yml`

## 获得帮助

加入 [我们的 Discord](https://discord.gg/zRDb35jfrt) 即可获得帮助。
