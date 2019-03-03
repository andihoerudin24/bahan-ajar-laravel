<template>
<div class="container">
     <v-form @submit.prevent="savetransaksi">
    <div class="row justify-content-center">
        <div class="col-md-12">
            <div class="card">
                <div class="card-header"><i class="fas fa-money-check-alt"> TRANSAKSI TIKET </i></div>
                    <div class="card-body">
                    <h3><i class="fab fa-wpforms"> Form Transaksi </i></h3>
                    <table class="table table-bordered">
                           <tr><td>
                                <div class="col-md-12">
                                    <label>Name Tiket</label>
                                      <v-flex xs12 sm12 d-flex>
                                        <select class="form-control">

                                        </select>
                                      </v-flex>
                                </div>
                           </td></tr>
                        <tr><td>
                                <div class="col-md-12">
                                    <label>Qty</label>
                                      <v-flex xs12 sm12 d-flex>
                                         <input  type="number" class="form-control">
                                      </v-flex>
                                </div>
                         </td></tr>
                          <tr><td>
                                <v-btn color="primary" type="submit" dark> Save
                                        <v-icon dark right>check_circle</v-icon>
                                </v-btn>
                                <v-btn color="primary" @click="finis()" dark> Finish
                                        <v-icon dark right>check_circle</v-icon>
                                </v-btn>
                                    <v-btn @click="print()" color="indigo" dark>Print
                                        <v-icon dark>backup</v-icon>
                                    </v-btn>
                            </td></tr>
                    </table>
                        <div class="card-header">
                           <i class="fab fa-wpforms"> Detail Transaksi </i>
                       </div>
                     <table class="table table-bordered">
                         <th>
                             <i class="fas fa-file-signature">  Nama Tiket </i>
                         </th>
                         <th>
                             <i class="fab fa-wolf-pack-battalion"> Qty </i></th>
                        <th>
                            <i class="fas fa-hand-holding-usd"> Harga Tiket </i>
                        </th>
                        <th>
                            <i class="fas fa-dollar-sign"> Subtotal  </i></th>
                            <th><i class="fas fa-ban"> Cancel </i>
                         </th>
                        <tr>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                               <td>
                                     <v-btn icon small>
                                            <v-icon color="red">cancel</v-icon>
                                     </v-btn>
                               </td>
                        </tr>
                    </table>
                </div>
            </div>
        </div>
    </div>
    </v-form>
</div>
</template>
