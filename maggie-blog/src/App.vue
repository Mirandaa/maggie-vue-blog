<template>
  <div id="app">
    <div class="layout">
      <Layout>
        <Header breakpoint>
          <Menu mode="horizontal" theme="dark" active-name="1">
            <div class="layout-logo"></div>
            <div class="layout-nav">
              <MenuItem name="1">
                <Icon type="ios-paper" />
                Home
              </MenuItem>
              <MenuItem name="2">
                <Icon type="ios-people" />
                Blog
              </MenuItem>
              <MenuItem name="4">
                <Icon type="ios-construct" />
                Settings
              </MenuItem>
            </div>

          </Menu>
        </Header>

        <Footer id="footer">
          <div class="inner">
            <section>
              <h2>About</h2>
              <div>
                2019 &copy; Maggie | Code | Design
              </div>
            </section>
            <section>
              <h2>Follow</h2>
              <div>
                2019 &copy; Maggie | Code | Design
              </div>
            </section>
            <ul class="copyright">
              <li>2019 © Maggie. All rights reserved</li>
              <li>Design: Maggie</li>
              <li></li>
            </ul>
          </div>
        </Footer>
      </Layout>
    </div>
    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {

    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

h2{
    font-size: 1.1em;
    font-weight: 900;
    line-height: 1.5;
    margin: 0 0 2em 0;
    text-transform: uppercase;
    letter-spacing: 0.35em;
}

.layout{
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    overflow: hidden;
}
.layout-logo{
    width: 100px;
    height: 30px;
    background: #5b6270;
    border-radius: 3px;
    float: left;
    position: relative;
    top: 15px;
    left: 20px;
}

.layout-nav{
    width: 420px;
    margin: 0 auto;
    margin-right: 20px;
}

#footer{
    background-color: #f6f6f6;
    border: 0;
    padding: 5em 0 3em 0;
    text-align: center;
    display: block;
}

#footer > .inner{
    width: 100%;
    max-width: 78em;
    margin: 0 auto;
    padding: 0 2.5em;
    flex-direction: row;
}

/*@media screen and (max-width: 1280px)*/
#footer > .inner section:nth-child(1) {
    width: calc(66% - 2.5em);
    margin-right: 2.5em;
}

#footer > .inner section:nth-child(2) {
    width: calc(33% - 1.25em);
    margin-left: 1.25em;
}

ul {
    display: block;
    margin: 0 0 2em 0;
}

#footer > .inner .copyright {
    float: left;
    width: 100%;
    padding: 0;
    margin-top: 5em;
    list-style: none;
    font-size: 0.8em;
    color: rgba(88, 88, 88, 0.5);
}

#footer > .inner .copyright li {
    display: inline-block;
    border-left: solid 1px rgba(88, 88, 88, 0.15);
    line-height: 1;
    padding: 0 0 0 1em;
    margin: 0 0 0 1em;
}

#footer > .inner .copyright li:first-child {
    border-left: 0;
    padding-left: 0;
    margin-left: 0;
}

</style>
