<template>
  <div id="app">
    <v-app id="inspire">
      <v-content>
        <v-container fluid fill-height>
          <v-layout align-center justify-center>
            <v-flex xs12 sm8 md4>
              <v-card class="elevation-12">
                <v-toolbar dark color="primary">
                  <v-toolbar-title>Đăng ký</v-toolbar-title>
                  <v-spacer></v-spacer>
                </v-toolbar>
                <v-card-text>
                  <v-form>
                    <v-text-field
                      prepend-icon="person"
                      name="login"
                      label="Tên đăng nhập"
                      type="text"
                    ></v-text-field>
                    <v-text-field
                      prepend-icon="lock"
                      name="password"
                      label="Mật khẩu"
                      id="password"
                      type="password"
                    ></v-text-field>
                    <v-text-field
                      prepend-icon="lock"
                      name="password"
                      label="Nhập lại mật khẩu"
                      id="password"
                      type="password"
                    ></v-text-field>
                    <v-text-field
                      prepend-icon="home"
                      name="password"
                      label="Trường dang học"
                      id="password"
                      type="password"
                    ></v-text-field>
                    <v-text-field
                      prepend-icon="mdi-calendar"
                      name="password"
                      label="Năm sinh"
                      id="password"
                      type="number"
                    ></v-text-field>
                    <v-radio-group v-model="select" label="Bạn là">
                      <v-radio label="Người cho thuê" value="1"></v-radio>
                      <v-radio label="Người muốn thuê" value="2"></v-radio>
                    </v-radio-group>
                  </v-form>
                </v-card-text>
                <v-card-actions>
                  <v-spacer></v-spacer>
                  <v-btn color="primary">Đăng nhập</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </v-content>
    </v-app>
  </div>
</template>
<script>
export default {
  data: () => ({
    drawer: null,
    select: 1
  })
};
</script>

<style>
</style>
