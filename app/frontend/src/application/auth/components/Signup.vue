<template>
  <div class="app flex-row align-items-center">
    <div class="container">
      <b-row class="justify-content-center">
        <b-col md="6" sm="8">
          <b-card no-body class="mx-4">
            <b-card-body class="p-4">
              <h1>Conta</h1>
              <p class="text-muted">Criar conta para eReports</p>
              <div class="input-group mb-3">
                <span class="input-group-addon"><i class="icon-user"></i></span>
                <input type="text" class="form-control" placeholder="Username">
              </div>

              <div class="input-group mb-3">
                <span class="input-group-addon"><i class="icon-people"></i></span>
                <input type="text" class="form-control" placeholder="Nome completo">
              </div>

              <div class="input-group mb-3">
                <span class="input-group-addon">@</span>
                <input type="text" class="form-control" placeholder="Email">
              </div>

              <div class="input-group mb-3">
                <span class="input-group-addon"><i class="icon-lock"></i></span>
                <input type="password" class="form-control" placeholder="Password">
              </div>

              <div class="input-group mb-4">
                <span class="input-group-addon"><i class="icon-lock"></i></span>
                <input type="password" class="form-control" placeholder="Repeat password">
              </div>

              <b-button variant="success" block>Criar Conta</b-button>

              <div class="text-right">
                <b-button variant="link" @click="login" class="px-0">Já possui conta?</b-button>
              </div>

            </b-card-body>
            <!--<b-card-footer class="p-4">
              <b-row>
                <b-col cols="6">
                  <b-button block class="btn btn-facebook"><span>facebook</span></b-button>
                </b-col>
                <b-col cols="6">
                  <b-button block class="btn btn-twitter" type="button"><span>twitter</span></b-button>
                </b-col>
              </b-row>
            </b-card-footer>-->
          </b-card>
        </b-col>
      </b-row>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Register',
  methods: {
    login () {
      this.$router.push('/auth/signin')
    }
  },
  mounted () {
  }
}
</script>
