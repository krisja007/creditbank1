<template>
    <div>
        <v-container class="grey lighten-5">
            <h1 class="text-center"> สมัครเรียนแบบบุคคลภายนอก Credit Bank กับมหาวิทยาลัยแม่โจ้</h1>
            <v-row no-gutter >
                <v-col  cols="3">
                    <v-card-title outline >
                        <v-autocomplete filled  outlined label="คำนำหน้าชื่อ" multiple> </v-autocomplete>
                    </v-card-title>
                </v-col> 
            </v-row>
            <v-row no-gutter>
                <v-col  cols="5">
                    <v-card-title outline >
                        <v-text-field filled  outlined label="ชื่อ-นามสกุล" ></v-text-field>
                    </v-card-title>
                </v-col> 

                <v-col  cols="5">
                    <v-card-title outline >
                        <v-text-field filled  outlined label="E-mail ที่สามารถติดต่อได้" multiple></v-text-field>
                    </v-card-title>
                </v-col> 
            </v-row>

            <v-row no-gutter >
                <v-col  cols="3" >
                <v-card-title outline >
                        <v-autocomplete solo-inverted label="ระดับการศึกษา" multiple></v-autocomplete>
                    </v-card-title>
                </v-col>

                <v-col  cols="5" offset="2">
                    <v-card-title outline >
                        <v-text-field filled  outlined label="เบอร์โทรศัพท์" multiple></v-text-field>
                    </v-card-title>
                </v-col> 
            </v-row>
            <v-row>
                <v-col  cols="5" >
                    <v-card-title outline >
                        <v-text-field filled  outlined label="ชื่อโรงเรียน" multiple></v-text-field>
                    </v-card-title>
                </v-col>
            </v-row>
             <p class="text-sm-left">กรุณาแนบไฟล์ (upload file) สำเนาบัตรประชาชน ที่มีลายเซ็นรับรองสำเนาถูกต้อง โดยสามารถใช้ไฟล์ pdf</p>
             <v-row no-gutter>
                <v-col cols="5"> <v-file-input  outlined> </v-file-input></v-col>
             </v-row>
             <p class="text-sm-left">กรุณาแนบไฟล์ (upload file) สำเนาบัตรทะเบียนบ้าน ที่มีลายเซ็นรับรองสำเนาถูกต้อง โดยสามารถใช้ไฟล์์  pdf</p>
             <v-row no-gutter>
                <v-col cols="5"> <v-file-input  outlined> </v-file-input></v-col>
             </v-row>
        
             <v-row no-gutter>
                <v-col cols="5">
                    <p class="text-sm-left">สมัครเรียน รายวิชาของคณะ (เลือกได้มากกว่า 1 คณะ)</p>
                </v-col>
             </v-row>

             <v-row>
                <v-col  cols="5">
                    <v-card-title outline >
                        <v-autocomplete solo-inverted label="รายชื่อคณะที่เปิดสอน" ></v-autocomplete>
                    </v-card-title>
                </v-col> 
                <v-col  cols="5">
                    <v-card-title outline >
                        <v-autocomplete solo-inverted label="รายวิชา และ วัน-เวลา" ></v-autocomplete>
                    </v-card-title>
                </v-col> 
             </v-row>

             <v-row>
                <v-col  cols="5">
                    <v-card-title outline >
                        <v-autocomplete solo-inverted label="เลือกรูปแบบการวัดผล" ></v-autocomplete>
                    </v-card-title>
                </v-col> 
             </v-row>

             <v-row>
                <v-col  cols="5" >
                    <v-card-title outline >
                        <v-text-field filled outlined  single-line  solo label="แจ้งข้อความเพิ่มเติม" multiple></v-text-field>
                    </v-card-title>
                </v-col>
             </v-row>
             <v-row>
                <v-col cols="12" sm="6" md="4"> <v-btn justify-center depressed color="success" @click="Register"> สมัครเรียน</v-btn></v-col>
             </v-row>
            
        </v-container>
    </div>    
</template>

<script setup>
</script>

<style scoped></style>