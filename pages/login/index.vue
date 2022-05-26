<template>
     <div class="h-screen w-screen flex justify-center items-center bg-corporateLight">
          <div class="glossyEffect md:w-3/12 px-10 pt-10 pb-8">
               <form>
                    <div class="mx-auto space-y-6">
                         <h5 class="text-center text-transparent text-2xl font-bold bg-clip-text text-corporate">Login Here</h5>
                         <customInput :id="'email'" :type="'email'" :placeholder="'Email'" :lableName="'Email'"/>
                         <customInput :id="'password'" :type="'password'" :placeholder="'Password'" :lableName="'Password'"/>

                         <div class="flex justify-between">
                              <NuxtLink to="#" class="text-corporateGray underline hover:decoration-corporate ">Forgot Password?</NuxtLink>
                              <button type="submit" class="customBtn uppercase">Login</button>
                         </div>
                         <h5 class="text-center text-sm">New User? <NuxtLink to="/sign-up" class="text-corporate underline hover:decoration-corporate uppercase">sign up</NuxtLink></h5>
                    </div>
               </form>
          </div>
     </div>
</template>

<script>
export default {

}
</script>

<style scoped>

</style>